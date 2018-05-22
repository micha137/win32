﻿---
Description: Functions
ms.assetid: '3D60C81F-B1CC-4485-B7C3-B1C6E903865B'
title: Functions
---

# Functions

## In this section



| Function                                                                                                | Description                                                                                                                                                                                                                                                                                                      |
|---------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**CoDecodeProxy**](codecodeproxy.md)<br/>                                                       | Locates the implementation of a Component Object Model (COM) interface in a server process given an interface to a proxied object.<br/>                                                                                                                                                                    |
| [**CreateControlInput**](createcontrolinput.md)<br/>                                             | Creates a [**ICoreInputSourceBase**](w_ui_core.icoreinputsourcebase) object in the caller’s UI thread.<br/>                                                                                                                                                                                                |
| [**CreateControlInputEx**](createcontrolinputex.md)<br/>                                         | Creates a [**ICoreInputSourceBase**](w_ui_core.icoreinputsourcebase) object in a worker thread or the UI thread. <br/>                                                                                                                                                                                     |
| [**CreateRandomAccessStreamOnFile**](createrandomaccessstreamonfile.md)<br/>                     | Creates a Windows Runtime random access stream for a file.<br/>                                                                                                                                                                                                                                            |
| [**CreateRandomAccessStreamOverStream**](createrandomaccessstreamoverstream.md)<br/>             | Creates a Windows Runtime random access stream around an [**IStream**](stg.istream) base implementation.<br/>                                                                                                                                                                                              |
| [**CreateStreamOverRandomAccessStream**](createstreamoverrandomaccessstream.md)<br/>             | Creates an [**IStream**](stg.istream) around a Windows Runtime [**IRandomAccessStream**](irandomaccessstream.md) object.<br/>                                                                                                                                                                             |
| [**CreateXamlUIPresenter**](createxamluipresenter.md)<br/>                                       | A static creator function that can create a [**XamlUIPresenter**](w_ui_xaml_hosting.xamluipresenter) for a render surface in a desktop app.<br/>                                                                                                                                                           |
| [**DbgRaiseAssertionFailure**](dbgraiseassertionfailure.md)<br/>                                 | Raises an assert for debugging. <br/>                                                                                                                                                                                                                                                                      |
| [**GetRestrictedErrorInfo**](getrestrictederrorinfo.md)<br/>                                     | Gets the restricted error information object set by a previous call to [**SetRestrictedErrorInfo**](setrestrictederrorinfo.md) in the current logical thread.<br/>                                                                                                                                        |
| [**HSTRING\_UserFree**](hstring-userfree.md)<br/>                                                | Frees resources on the server side when called by RPC stub files.<br/>                                                                                                                                                                                                                                     |
| [**HSTRING\_UserFree64**](hstring-userfree64.md)<br/>                                            | Frees resources on the server side when called by RPC stub files. <br/>                                                                                                                                                                                                                                    |
| [**HSTRING\_UserMarshal**](hstring-usermarshal.md)<br/>                                          | Marshals an [**HSTRING**](hstring.md) object into the RPC buffer.<br/>                                                                                                                                                                                                                                    |
| [**HSTRING\_UserMarshal64**](hstring-usermarshal64.md)<br/>                                      | Marshals an [**HSTRING**](hstring.md) object into the RPC buffer.<br/>                                                                                                                                                                                                                                    |
| [**HSTRING\_UserSize**](hstring-usersize.md)<br/>                                                | Calculates the wire size of the [**HSTRING**](hstring.md) object, and gets its handle and data.<br/>                                                                                                                                                                                                      |
| [**HSTRING\_UserSize64**](hstring-usersize64.md)<br/>                                            | Calculates the wire size of the [**HSTRING**](hstring.md) object, and gets its handle and data.<br/>                                                                                                                                                                                                      |
| [**HSTRING\_UserUnmarshal**](hstring-userunmarshal.md)<br/>                                      | Unmarshals an [**HSTRING**](hstring.md) object from the RPC buffer.<br/>                                                                                                                                                                                                                                  |
| [**HSTRING\_UserUnmarshal64**](hstring-userunmarshal64.md)<br/>                                  | Unmarshals an [**HSTRING**](hstring.md) object from the RPC buffer.<br/>                                                                                                                                                                                                                                  |
| [**IsErrorPropagationEnabled**](iserrorpropagationenabled.md)<br/>                               | Indicates whether the [**CoreApplication.UnhandledErrorDetected**](w_appmod_core.coreapplication_unhandlederrordetected) event occurs for the errors that are returned by the delegate registered as a callback function for a Windows Runtime API event or the completion of an asynchronous method.<br/> |
| [**DllGetActivationFactory**](dllgetactivationfactory.md)<br/>                                   | Retrieves the activation factory from a DLL that contains activatable Windows Runtime classes.<br/>                                                                                                                                                                                                        |
| [**MetaDataGetDispenser**](metadatagetdispenser.md)<br/>                                         | Creates a dispenser class.<br/>                                                                                                                                                                                                                                                                            |
| [**PdfCreateRenderer**](pdfcreaterenderer.md)<br/>                                               | Gets an instance of the [**IPdfRendererNative**](ipdfrenderernative.md) interface for displaying a single page of a Portable Document Format (PDF) file.<br/>                                                                                                                                             |
| [**PdfRenderParams**](pdfrenderparams.md)<br/>                                                   | Populates a [**PDF\_RENDER\_PARAMS**](pdf-render-params.md) stucture. A PDF\_RENDER\_PARAMS structure represents a set of properties for outputting a single page of a PDF file.<br/>                                                                                                                     |
| [**RoActivateInstance**](roactivateinstance.md)<br/>                                             | Activates the specified Windows Runtime class.<br/>                                                                                                                                                                                                                                                        |
| [**RoCaptureErrorContext**](rocaptureerrorcontext.md)<br/>                                       | Saves the current error context so that it's available for later calls to the [**RoFailFastWithErrorContext**](rofailfastwitherrorcontext.md) function.<br/>                                                                                                                                              |
| [**RoClearError**](roclearerror.md)<br/>                                                         | Removes existing error information from the current thread environment block (TEB).<br/>                                                                                                                                                                                                                   |
| [**RoFailFastWithErrorContext**](rofailfastwitherrorcontext.md)<br/>                             | Raises a non-continuable exception in the current process.<br/>                                                                                                                                                                                                                                            |
| [**RoFreeParameterizedTypeExtra**](rofreeparameterizedtypeextra.md)<br/>                         | Frees the handle allocated by [**RoGetParameterizedTypeInstanceIID**](rogetparameterizedtypeinstanceiid.md).<br/>                                                                                                                                                                                         |
| [**RoGetActivatableClassRegistration**](rogetactivatableclassregistration.md)<br/>               | Enables retrieving class registration information.<br/>                                                                                                                                                                                                                                                    |
| [**RoGetActivationFactory**](rogetactivationfactory.md)<br/>                                     | Gets the activation factory for the specified runtime class.<br/>                                                                                                                                                                                                                                          |
| [**RoGetAgileReference**](rogetagilereference.md)<br/>                                           | Creates an agile reference for an object specified by the given interface.<br/>                                                                                                                                                                                                                            |
| [**RoGetApartmentIdentifier**](rogetapartmentidentifier.md)<br/>                                 | Gets a unique identifier for the current apartment.<br/>                                                                                                                                                                                                                                                   |
| [**RoGetBufferMarshaler**](rogetbuffermarshaler.md)<br/>                                         | Provides a standard IBuffer marshaler to implement the semantics associated with the IBuffer interface when it is marshaled.<br/>                                                                                                                                                                          |
| [**RoGetErrorReportingFlags**](rogeterrorreportingflags.md)<br/>                                 | Gets the current reporting behavior of Windows Runtime error functions.<br/>                                                                                                                                                                                                                               |
| [**RoGetMetaDataFile**](rogetmetadatafile.md)<br/>                                               | Locates and retrieves the metadata file that describes the Application Binary Interface (ABI) for the specified typename.<br/>                                                                                                                                                                             |
| [**RoGetParameterizedTypeInstanceIID**](rogetparameterizedtypeinstanceiid.md)<br/>               | Computes the interface identifier (IID) of the interface or delegate type that results when a parameterized interface or delegate is instantiated with the specified type arguments.<br/>                                                                                                                  |
| [**RoGetServerActivatableClasses**](rogetserveractivatableclasses.md)<br/>                       | Retrieves the activatable classes that are registered for a given executable (EXE) server, which was registered under the package ID of the calling process.<br/>                                                                                                                                          |
| [**RoInitialize**](roinitialize.md)<br/>                                                         | Initializes the Windows Runtime on the current thread with the specified concurrency model.<br/>                                                                                                                                                                                                           |
| [**RoInspectThreadErrorInfo**](roinspectthreaderrorinfo.md)<br/>                                 | Gets the error object that represents the call stack at the point where the error originated<br/>                                                                                                                                                                                                          |
| [**RoInspectCapturedStackBackTrace**](roinspectcapturedstackbacktrace.md)<br/>                   | Provides a way to for debuggers to inspect a call stack from a target process.<br/>                                                                                                                                                                                                                        |
| [**RoOriginateError**](rooriginateerror.md)<br/>                                                 | Reports an error and an informative string to an attached debugger.<br/>                                                                                                                                                                                                                                   |
| [**RoOriginateErrorW**](rooriginateerrorw.md)<br/>                                               | Reports an error and an informative string to an attached debugger.<br/>                                                                                                                                                                                                                                   |
| [**RoOriginateLanguageException**](rooriginatelanguageexception.md)<br/>                         | Reports an error, an informative string, and an error object to an attached debugger.<br/>                                                                                                                                                                                                                 |
| [**RoParameterizedTypeExtraGetTypeSignature**](roparameterizedtypeextragettypesignature.md)<br/> | Gets the type signature used to compute the IID from the last call to [**RoGetParameterizedTypeInstanceIID**](rogetparameterizedtypeinstanceiid.md) with the specified handle.<br/>                                                                                                                       |
| [**RoParseTypeName**](roparsetypename.md)<br/>                                                   | Parses a type name and existing type parameters, in the case of parameterized types.<br/>                                                                                                                                                                                                                  |
| [**RoRegisterActivationFactories**](roregisteractivationfactories.md)<br/>                       | Registers an array out-of-process activation factories for a Windows Runtime exe server.<br/>                                                                                                                                                                                                              |
| [**RoRegisterForApartmentShutdown**](roregisterforapartmentshutdown.md)<br/>                     | Registers an [**IApartmentShutdown**](iapartmentshutdown.md) callback to be invoked when the current apartment shuts down.<br/>                                                                                                                                                                           |
| [**RoReportUnhandledError**](roreportunhandlederror.md)<br/>                                     | Triggers the Global Error Handler when an unhandled exception occurs.<br/>                                                                                                                                                                                                                                 |
| [**RoReportFailedDelegate**](roreportfaileddelegate.md)<br/>                                     | Triggers the Global Error Handler when a delegate failure occurs.<br/>                                                                                                                                                                                                                                     |
| [**RoResolveNamespace**](roresolvenamespace.md)<br/>                                             | Determine the direct children, types, and sub-namespaces of the specified Windows Runtime namespace, from any programming language supported by the Windows Runtime.<br/>                                                                                                                                  |
| [**RoResolveRestrictedErrorInfoReference**](roresolverestrictederrorinforeference.md)<br/>       | Returns the [**IRestrictedErrorInfo**](irestrictederrorinfo.md) interface pointer based on the given reference.<br/>                                                                                                                                                                                      |
| [**RoRevokeActivationFactories**](rorevokeactivationfactories.md)<br/>                           | Removes an array of registered activation factories from the Windows Runtime.<br/>                                                                                                                                                                                                                         |
| [**RoSetErrorReportingFlags**](roseterrorreportingflags.md)<br/>                                 | Sets the reporting behavior of Windows Runtime error functions.<br/>                                                                                                                                                                                                                                       |
| [**RoTransformError**](rotransformerror.md)<br/>                                                 | Reports a modified error and an informative string to an attached debugger.<br/>                                                                                                                                                                                                                           |
| [**RoTransformErrorW**](rotransformerrorw.md)<br/>                                               | Reports a transformed error and an informative string to an attached debugger.<br/>                                                                                                                                                                                                                        |
| [**RoUninitialize**](rouninitialize.md)<br/>                                                     | Closes the Windows Runtime on the current thread.<br/>                                                                                                                                                                                                                                                     |
| [**RoUnregisterForApartmentShutdown**](rounregisterforapartmentshutdown.md)<br/>                 | Unregisters a previously registered [**IApartmentShutdown**](iapartmentshutdown.md) interface.<br/>                                                                                                                                                                                                       |
| [**SetRestrictedErrorInfo**](setrestrictederrorinfo.md)<br/>                                     | Sets the restricted error information object for the current thread.<br/>                                                                                                                                                                                                                                  |
| [**WindowsCompareStringOrdinal**](windowscomparestringordinal.md)<br/>                           | Compares two specified [**HSTRING**](hstring.md) objects and returns an integer that indicates their relative position in a sort order.<br/>                                                                                                                                                              |
| [**WindowsConcatString**](windowsconcatstring.md)<br/>                                           | Concatenates two specified strings.<br/>                                                                                                                                                                                                                                                                   |
| [**WindowsCreateString**](windowscreatestring.md)<br/>                                           | Creates a new [**HSTRING**](hstring.md) based on the specified source string.<br/>                                                                                                                                                                                                                        |
| [**WindowsCreateStringReference**](windowscreatestringreference.md)<br/>                         | Creates a new string reference based on the specified string.<br/>                                                                                                                                                                                                                                         |
| [**WindowsDeleteString**](windowsdeletestring.md)<br/>                                           | Decrements the reference count of a string buffer.<br/>                                                                                                                                                                                                                                                    |
| [**WindowsDeleteStringBuffer**](windowsdeletestringbuffer.md)<br/>                               | Discards a preallocated string buffer if it was not promoted to an [**HSTRING**](hstring.md).<br/>                                                                                                                                                                                                        |
| [**WindowsDuplicateString**](windowsduplicatestring.md)<br/>                                     | Creates a copy of the specified string.<br/>                                                                                                                                                                                                                                                               |
| [**WindowsGetStringLen**](windowsgetstringlen.md)<br/>                                           | Gets the length, in Unicode characters, of the specified string.<br/>                                                                                                                                                                                                                                      |
| [**WindowsGetStringRawBuffer**](windowsgetstringrawbuffer.md)<br/>                               | Gets the backing buffer for the specified string.<br/>                                                                                                                                                                                                                                                     |
| [**WindowsInspectString**](windowsinspectstring.md)<br/>                                         | Provides a way to for debuggers to display the value of an Windows Runtime [**HSTRING**](hstring.md) in another address space, remotely, or from a dump. <br/>                                                                                                                                            |
| [**WindowsInspectString2**](windowsinspectstring2.md)<br/>                                       | Provides a way to for debuggers to display the value of an Windows Runtime [**HSTRING**](hstring.md) in another address space, remotely, or from a dump. <br/>                                                                                                                                            |
| [**WindowsIsStringEmpty**](windowsisstringempty.md)<br/>                                         | Indicates whether the specified string is the empty string.<br/>                                                                                                                                                                                                                                           |
| [**WindowsPreallocateStringBuffer**](windowspreallocatestringbuffer.md)<br/>                     | Allocates a mutable character buffer for use in [**HSTRING**](hstring.md) creation.<br/>                                                                                                                                                                                                                  |
| [**WindowsPromoteStringBuffer**](windowspromotestringbuffer.md)<br/>                             | Creates an [**HSTRING**](hstring.md) from the specified [**HSTRING\_BUFFER**](hstring-buffer.md).<br/>                                                                                                                                                                                                   |
| [**WindowsReplaceString**](windowsreplacestring.md)<br/>                                         | Replaces all occurrences of a set of characters in the specified string with another set of characters to create a new string.<br/>                                                                                                                                                                        |
| [**WindowsStringHasEmbeddedNull**](windowsstringhasembeddednull.md)<br/>                         | Indicates whether the specified string has embedded null characters.<br/>                                                                                                                                                                                                                                  |
| [**WindowsSubstring**](windowssubstring.md)<br/>                                                 | Retrieves a substring from the specified string. The substring starts at the specified character position.<br/>                                                                                                                                                                                            |
| [**WindowsSubstringWithSpecifiedLength**](windowssubstringwithspecifiedlength.md)<br/>           | Retrieves a substring from the specified string. The substring starts at a specified character position and has a specified length.<br/>                                                                                                                                                                   |
| [**WindowsTrimStringEnd**](windowstrimstringend.md)<br/>                                         | Removes all trailing occurrences of a specified set of characters from the source string.<br/>                                                                                                                                                                                                             |
| [**WindowsTrimStringStart**](windowstrimstringstart.md)<br/>                                     | Removes all leading occurrences of a specified set of characters from the source string.<br/>                                                                                                                                                                                                              |



 

 

 



