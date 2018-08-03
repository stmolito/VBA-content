---
title: QueryTable.TextFileConsecutiveDelimiter Property (Excel)
keywords: vbaxl10.chm518102
f1_keywords:
- vbaxl10.chm518102
ms.prod: excel
api_name:
- Excel.QueryTable.TextFileConsecutiveDelimiter
ms.assetid: 2d86ba86-9601-9a2d-0cee-4648d77dab2c
ms.date: 06/08/2017
---


# QueryTable.TextFileConsecutiveDelimiter Property (Excel)

 **True** if consecutive delimiters are treated as a single delimiter when you import a text file into a query table. The default value is **False** . Read/write **Boolean** .


## Syntax

 _expression_ . **TextFileConsecutiveDelimiter**

 _expression_ A variable that represents a **QueryTable** object.


## Remarks

Use this property is only when your query table is based on data from a text file (with the  **[QueryType](querytable-querytype-property-excel.md)** property set to **xlTextImport** ), and only if the value of the **[TextFileParseType](querytable-textfileparsetype-property-excel.md)** property is **xlDelimited** .

If you import data using the user interface, data from a Web query or a text query is imported as a  **[QueryTable](querytable-object-excel.md)** object, while all other external data is imported as a **[ListObject](listobject-object-excel.md)** object.

If you import data using the object model, data from a Web query or a text query must be imported as a  **QueryTable** , while all other external data can be imported as either a **ListObject** or a **QueryTable** .

The  **TextFileConsecutiveDelimiter** property applies only to **QueryTable** objects.


## Example

This example sets the space character to be the delimiter in the query table on the first worksheet in the first workbook, and then it refreshes the query table. Consecutive spaces are treated as a single delimiter.


```vb
Set shFirstQtr = Workbooks(1).Worksheets(1) 
Set qtQtrResults = shFirstQtr.QueryTables _ 
 .Add(Connection := "TEXT;C:\My Documents\19980331.txt", _ 
 Destination := shFirstQtr.Cells(1, 1)) 
With qtQtrResults 
 .TextFileParseType = xlDelimited 
 .TextFileSpaceDelimiter = True 
 .TextFileConsecutiveDelimiter = True 
 .Refresh 
End With
```


## See also


#### Concepts


[QueryTable Object](querytable-object-excel.md)

