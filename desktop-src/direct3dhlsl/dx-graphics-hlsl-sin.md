---
title: sin
description: Returns the sine of the specified value.
ms.assetid: 'e1c3ead8-73dd-4798-8553-1a42dbaefe8e'
keywords: ["sin HLSL"]
topic_type:
- apiref
api_name:
- sin
api_type:
- NA
---

# sin

Returns the sine of the specified value.



| *ret* sin(*x*) |
|----------------|



�

## Parameters



| Item                                                   | Description                                        |
|--------------------------------------------------------|----------------------------------------------------|
| <span id="x"></span><span id="X"></span>*x*<br/> | \[in\] The specified value, in radians.<br/> |



�

## Return Value

The sine of the *x* parameter.

## Type Description



| Name  | [**Template Type**](dx-graphics-hlsl-intrinsic-functions.md)                                                  | [**Component Type**](dx-graphics-hlsl-intrinsic-functions.md) | Size                           |
|-------|----------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------|--------------------------------|
| *x*   | [**scalar**](dx-graphics-hlsl-intrinsic-functions.md#component-and-template-types), **vector**, or **matrix** | [**float**](https://msdn.microsoft.com/library/windows/desktop/aa383751)                        | any                            |
| *ret* | same as input *x*                                                                                              | [**float**](https://msdn.microsoft.com/library/windows/desktop/aa383751)                        | same dimension(s) as input *x* |



�

## Minimum Shader Model

This function is supported in the following shader models.



| Shader Model                                                                       | Supported           |
|------------------------------------------------------------------------------------|---------------------|
| [Shader Model 2 (DirectX HLSL)](dx-graphics-hlsl-sm2.md) and higher shader models | yes                 |
| [Shader Model 1 (DirectX HLSL)](dx-graphics-hlsl-sm1.md)                          | yes (vs\_1\_1 only) |



�

## See also

<dl> <dt>

[**Intrinsic Functions (DirectX HLSL)**](dx-graphics-hlsl-intrinsic-functions.md)
</dt> </dl>

�

�




