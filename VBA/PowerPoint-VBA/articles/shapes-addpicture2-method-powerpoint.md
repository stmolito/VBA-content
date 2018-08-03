---
title: Shapes.AddPicture2 Method (PowerPoint)
ms.assetid: 2956fa14-40bb-458a-aef1-caceab15e067
ms.date: 06/08/2017
ms.prod: powerpoint
---


# Shapes.AddPicture2 Method (PowerPoint)

Creates a picture from an existing file. Returns a  **[Shape](shape-object-powerpoint.md)** object that represents the new picture.


## Syntax

 _expression_. **AddPicture2**( **_FileName_**, **_LinkToFile_**, **_SaveWithDocument_**, **_Left_**, **_Top_**, **_Width_**, **_Height_**, **_compress_** )

 _expression_ A variable that represents a **Shapes** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _FileName_|Required|**String**|The file from which the OLE object is to be created.|
| _LinkToFile_|Required|**[MsoTriState](http://msdn.microsoft.com/library/2036cfc9-be7d-e05c-bec7-af05e3c3c515%28Office.15%29.aspx)**|Determines whether the picture will be linked to the file from which it was created.|
| _SaveWithDocument_|Required|**[MsoTriState](http://msdn.microsoft.com/library/2036cfc9-be7d-e05c-bec7-af05e3c3c515%28Office.15%29.aspx)**|Determines whether the linked picture will be saved with the document into which it is inserted. This argument must be  **msoTrue** if _LinkToFile_ is **msoFalse**.|
| _Left_|Required|**Single**|The position, measured in points, of the left edge of the picture relative to the left edge of the slide.|
| _Top_|Required|**Single**|The position, measured in points, of the top edge of the picture relative to the top edge of the slide.|
| _Width_|Optional|**Single**|The width of the picture, measured in points.|
| _Height_|Optional|**Single**|The height of the picture, measured in points.|
| _compress_|Optional|[MsoPictureCompress](http://msdn.microsoft.com/library/f58e84f7-f284-425f-88df-b8f8578cebeb%28Office.15%29.aspx)|Determines whether the picture should be compressed when inserted.|

### Return Value

Shape


## See also


#### Concepts


[Shapes Object](shapes-object-powerpoint.md)

