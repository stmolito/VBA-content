---
title: Document.Tables Property (Word)
keywords: vbawd10.chm158007302
f1_keywords:
- vbawd10.chm158007302
ms.prod: word
api_name:
- Word.Document.Tables
ms.assetid: a0e09aff-af98-5d10-ba49-01ba6fcfa2d1
ms.date: 06/08/2017
---


# Document.Tables Property (Word)

Returns a  **[Table](table-object-word.md)** collection that represents all the tables in the specified document. Read-only.


## Syntax

 _expression_ . **Tables**

 _expression_ A variable that represents a **[Document](document-object-word.md)** object.


## Remarks

For information about returning a single member of a collection, see [Returning an Object from a Collection](http://msdn.microsoft.com/library/28f76384-f495-9640-a7c8-10ada3fac727%28Office.15%29.aspx).


## Example

This example creates a 5x5 table in the active document and then applies a predefined format to it.


```vb
Selection.Collapse Direction:=wdCollapseStart 
Set myTable = ActiveDocument.Tables.Add(Range:=Selection.Range, _ 
NumRows:=5, NumColumns:=5) 
myTable.AutoFormat Format:=wdTableFormatClassic2
```

This example inserts numbers and text into the first column of the first table in the active document.




```vb
num = 90 
For Each acell In ActiveDocument.Tables(1).Columns(1).Cells 
 acell.Range.Text = num &; " Sales" 
 num = num + 1 
Next acell
```


## See also


#### Concepts


[Document Object](document-object-word.md)

