---
title: SetExportPath method of the Win32\_RDMSDeploymentSettings class
description: Updates the directory path to which virtual machines are deployed for a virtual desktop collection.
audience: developer
author: REDMOND\\markl
manager: REDMOND\\markl
ms.assetid: 'e52b79c8-6724-4264-93d5-4a2a14c89b6b'
ms.prod: 'windows-server-dev'
ms.technology: 'remote-desktop-services'
ms.tgt_platform: multiple
keywords: ["SetExportPath method Remote Desktop Services", "SetExportPath method Remote Desktop Services , Win32_RDMSDeploymentSettings class", "Win32_RDMSDeploymentSettings class Remote Desktop Services , SetExportPath method"]
topic_type:
- apiref
api_name:
- Win32_RDMSDeploymentSettings.SetExportPath
api_location:
- RDMS.dll
api_type:
- COM
---

# SetExportPath method of the Win32\_RDMSDeploymentSettings class

Updates the directory path to which virtual machines are deployed for a virtual desktop collection.

## Syntax


```mof
uint32 SetExportPath(
  [in]�string DirectoryPath
);
```



## Parameters

<dl> <dt>

*DirectoryPath* \[in\]
</dt> <dd>

The new directory path.

</dd> </dl>

## Return value

Returns 0 on success, otherwise returns a WMI error code.

## Requirements



|                                     |                                                                                             |
|-------------------------------------|---------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | None supported<br/>                                                                   |
| Minimum supported server<br/> | Windows Server�2012<br/>                                                              |
| Namespace<br/>                | Root\\CIMv2\\rdms<br/>                                                                |
| MOF<br/>                      | <dl> <dt>RDManagement.mof</dt> </dl> |
| DLL<br/>                      | <dl> <dt>RDMS.dll</dt> </dl>         |



## See also

<dl> <dt>

[**Win32\_RDMSDeploymentSettings**](win32-rdmsdeploymentsettings.md)
</dt> </dl>

�

�




