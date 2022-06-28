---
uid: Manifest.Content.Protocols.Protocol.Version.Selection.Range
---

# Range element

Specifies a range.

## Type

[TypeNonEmptyString](xref:Manifest-TypeNonEmptyString)

## Parent

[Selection](xref:Manifest.Content.Protocols.Protocol.Version.Selection)

## Attributes

|Name|Type|Required|Description|
|--- |--- |--- |--- |
|[triggerPackagePipelineOnChange](xref:Manifest.Content.Protocols.Protocol.Version.Selection.Range-triggerPackagePipelineOnChange )|[EnumTrueFalse](xref:Manifest-EnumTrueFalse)|Yes|Specifies whether a change to this item should trigger the package pipeline chain.|
|[rangeSelection](xref:Manifest.Content.Protocols.Protocol.Version.Selection.Range-rangeSelection)|[EnumLatestReleaseLatestBuild](xref:Manifest-EnumLatestReleaseLatestBuild)|Yes|Specifies whether the last version of the range (if used) should be a release or if it can be a development (build) version.|