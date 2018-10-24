---
Description: This topic is not current. For the most current information, see the Print Schema Specification.
ms.assetid: e86d6a5d-484d-4c80-8c86-7d12d287ee21
title: PageMediaSizePSHeightOffset
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# PageMediaSizePSHeightOffset

This topic is not current. For the most current information, see the [Print Schema Specification](http://go.microsoft.com/?linkid=7141496).

Specifies the offset, parallel to the feed-orientation direction (Reference [PostScript Printer Description File Format Specification](http://go.microsoft.com/fwlink/p/?linkid=178075)).

-   [Element Information](#element-information)
-   [Structure Content](#structure-content)

## Element Information



| Name                       |                                                             |
|----------------------------|-------------------------------------------------------------|
| Element Type <br/>   | ParameterDef<br/>                                     |
| Scoping Prefix <br/> | Page<br/>                                             |
| Notes <br/>          | Linked to PageMediaSize element, CustomPS option<br/> |



 

## Structure Content

The XML structure of this element is:

``` syntax
<psf:ParameterDef name="psk:PageMediaSizePSHeightOffset">
  <psf:Property name="psf:DataType">
    <psf:Value xsi:type="xs:string">xs:integer</psf:Value>
  </psf:Property>
  <psf:Property name="psf:DefaultValue">
    <psf:Value xsi:type="xs:integer">_Undefined_</psf:Value>
  </psf:Property>
  <psf:Property name="psf:MaxValue">
    <psf:Value xsi:type="xs:integer">_Undefined_</psf:Value>
  </psf:Property>
  <psf:Property name="psf:MinValue">
    <psf:Value xsi:type="xs:integer">_Undefined_</psf:Value>
  </psf:Property>
  <psf:Property name="psf:Multiple">
    <psf:Value xsi:type="xs:integer">1</psf:Value>
  </psf:Property>
  <psf:Property name="psf:Mandatory">
    <psf:Value xsi:type="xs:string">psk:Conditional</psf:Value>
  </psf:Property>
  <psf:Property name="psf:UnitType">
    <psf:Value xsi:type="xs:string">microns</psf:Value>
  </psf:Property>
</psf:ParameterDef>
      
```

## Structure Properties

The following table outlines the characteristics of the variables defined in the XML structure.



| Property                | xsi:type           | Value                      |
|-------------------------|--------------------|----------------------------|
| DataType<br/>     | string<br/>  | xs:integer<br/>      |
| DefaultValue<br/> | integer<br/> | undefined<br/>       |
| MaxValue<br/>     | integer<br/> | undefined<br/>       |
| MinValue<br/>     | integer<br/> | undefined<br/>       |
| Mandatory<br/>    | string<br/>  | psk:Conditional<br/> |
| Multiple<br/>     | integer<br/> | 1<br/>               |
| UnitType<br/>     | string<br/>  | microns<br/>         |



 

## Related topics

<dl> <dt>

[PostScript Printer Description File Format Specification](http://go.microsoft.com/fwlink/p/?linkid=178075)
</dt> <dt>

[Print Schema Specification](http://go.microsoft.com/?linkid=7141496)
</dt> </dl>

 

 



