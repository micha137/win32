---
Description: Using the Source Resolver
ms.assetid: '94e2a411-96b8-4506-8491-78f4f5f286ce'
title: Using the Source Resolver
---

# Using the Source Resolver

The source resolver takes a URL or byte stream and creates the appropriate media source for that content. To create the source resolver, call [**MFCreateSourceResolver**](mfcreatesourceresolver.md). This function returns an [**IMFSourceResolver**](imfsourceresolver.md) interface pointer.

The source resolver has both synchronous and asynchronous methods. If you are using the source resolver from your main application thread, the asynchronous methods will make your user interface more responsive. The synchronous methods can block for a noticeable amount of time, particularly if the source resolver must open a network resource.

The synchronous methods are:

-   [**IMFSourceResolver::CreateObjectFromURL**](imfsourceresolver-createobjectfromurl.md)
-   [**IMFSourceResolver::CreateObjectFromByteStream**](imfsourceresolver-createobjectfrombytestream.md)

The asynchronous methods are:

-   [**IMFSourceResolver::BeginCreateObjectFromURL**](imfsourceresolver-begincreateobjectfromurl.md)
-   [**IMFSourceResolver::BeginCreateObjectFromByteStream**](imfsourceresolver-begincreateobjectfrombytestream.md)

For the asynchronous methods, each method has a corresponding **End...** method to complete the asynchronous request, and a **Cancel...** method to cancel a pending request. For more information about asynchronous methods in Media Foundation, see [Asynchronous Callback Methods](asynchronous-callback-methods.md).

The following code example creates a media source from a URL. This example uses the synchronous method.


```C++
//  Create a media source from a URL.
HRESULT CreateMediaSource(PCWSTR sURL, IMFMediaSource **ppSource)
{
    MF_OBJECT_TYPE ObjectType = MF_OBJECT_INVALID;

    IMFSourceResolver* pSourceResolver = NULL;
    IUnknown* pSource = NULL;

    // Create the source resolver.
    HRESULT hr = MFCreateSourceResolver(&amp;pSourceResolver);
    if (FAILED(hr))
    {
        goto done;
    }

    // Use the source resolver to create the media source.

    // Note: For simplicity this sample uses the synchronous method to create 
    // the media source. However, creating a media source can take a noticeable
    // amount of time, especially for a network source. For a more responsive 
    // UI, use the asynchronous BeginCreateObjectFromURL method.

    hr = pSourceResolver->CreateObjectFromURL(
        sURL,                       // URL of the source.
        MF_RESOLUTION_MEDIASOURCE,  // Create a source object.
        NULL,                       // Optional property store.
        &amp;ObjectType,        // Receives the created object type. 
        &amp;pSource            // Receives a pointer to the media source.
        );
    if (FAILED(hr))
    {
        goto done;
    }

    // Get the IMFMediaSource interface from the media source.
    hr = pSource->QueryInterface(IID_PPV_ARGS(ppSource));

done:
    SafeRelease(&amp;pSourceResolver);
    SafeRelease(&amp;pSource);
    return hr;
}
```



## Related topics

<dl> <dt>

[Source Resolver](source-resolver.md)
</dt> </dl>

 

 


