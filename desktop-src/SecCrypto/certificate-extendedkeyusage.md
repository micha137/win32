﻿---
Description: 'Returns an ExtendedKeyUsage object that indicates the valid uses of the certificate.'
ms.assetid: 'e974e9e2-1011-48b7-9ebc-e754e4990286'
title: 'ICertificate2::ExtendedKeyUsage method'
---

# ICertificate2::ExtendedKeyUsage method

\[CAPICOM is a 32-bit only component that is available for use in the following operating systems: Windows Server 2008, Windows Vista, and Windows XP. Instead, use the [**X509Certificate2 Class**](T:System.Security.Cryptography.X509Certificates.X509Certificate2) in the [**System.Security.Cryptography.X509Certificates**](frlrfSystemSecurityCryptographyX509Certificates) namespace.\]

The **ExtendedKeyUsage** method returns an [**ExtendedKeyUsage**](extendedkeyusage.md) object that indicates the valid uses of the certificate.

## Syntax


```VB
Certificate.ExtendedKeyUsage()
```



## Parameters

This method has no parameters.

## Return value

The [**ExtendedKeyUsage**](extendedkeyusage.md) object that is associated with the certificate.

## Requirements



|                                  |                                                                                        |
|----------------------------------|----------------------------------------------------------------------------------------|
| End of client support<br/> | Windows Vista<br/>                                                               |
| End of server support<br/> | Windows Server 2008<br/>                                                         |
| Redistributable<br/>       | CAPICOM 2.0 or later on Windows Server 2003 and Windows XP<br/>                  |
| DLL<br/>                   | <dl> <dt>Capicom.dll</dt> </dl> |



## See also

<dl> <dt>

[Cryptography Objects](cryptography-objects.md)
</dt> <dt>

[**Certificate**](certificate.md)
</dt> </dl>

 

 



