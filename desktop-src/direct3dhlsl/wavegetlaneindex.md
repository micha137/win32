---
title: WaveGetLaneIndex function
description: Returns the index of the current lane within the current wave.
ms.assetid: 'C05BD814-23DF-432F-8669-C03842B77AC7'
keywords: ["WaveGetLaneIndex function HLSL"]
topic_type:
- apiref
api_name:
- WaveGetLaneIndex
api_type:
- NA
---

# WaveGetLaneIndex function

Returns the index of the current lane within the current wave.

## Syntax

``` syntax
uint WaveGetLaneIndex(void);
```

## Parameters

This function has no parameters.

## Return value

The current lane index. The result will be between 0 and the result returned from [**WaveGetLaneCount**](wavegetlanecount.md).

## Remarks

This function is supported from shader model 6.0, in the following types of shaders:



| Vertex | Hull | Domain | Geometry | Pixel | Compute |
|--------|------|--------|----------|-------|---------|
|        |      |        |          | x     | x       |



 

## See also

<dl> <dt>

[Overview of Shader Model 6](hlsl-shader-model-6-0-features-for-direct3d-12.md)
</dt> <dt>

[Shader Model 6](shader-model-6-0.md)
</dt> </dl>

 

 



