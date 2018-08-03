---
title: Series.PictureType Property (Word)
keywords: vbawd10.chm123732129
f1_keywords:
- vbawd10.chm123732129
ms.prod: word
api_name:
- Word.Series.PictureType
ms.assetid: 29150e44-0815-9e6e-7fcb-92f030f3cf6a
ms.date: 06/08/2017
---


# Series.PictureType Property (Word)

Returns or sets a value that specifies how pictures are displayed on a column or bar picture chart. Read/write  **[XlChartPictureType](xlchartpicturetype-enumeration-word.md)** .


## Syntax

 _expression_ . **PictureType**

 _expression_ A variable that represents a **[Series](series-object-word.md)** object.


## Example

The following example sets series one of the first chart in the active document to stretch pictures. You should run the example on a 2-D column chart that has picture data markers.


```vb
With ActiveDocument.InlineShapes(1) 
 If .HasChart Then 
 .Chart.SeriesCollection(1).PictureType = xlStretch 
 End If 
End With
```


## See also


#### Concepts


[Series Object](series-object-word.md)

