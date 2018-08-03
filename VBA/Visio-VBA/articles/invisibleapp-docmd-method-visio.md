---
title: InvisibleApp.DoCmd Method (Visio)
keywords: vis_sdr.chm17516190
f1_keywords:
- vis_sdr.chm17516190
ms.prod: visio
api_name:
- Visio.InvisibleApp.DoCmd
ms.assetid: d38786e8-5511-a489-937a-4fb9cd3fc502
ms.date: 06/08/2017
---


# InvisibleApp.DoCmd Method (Visio)

Performs the command that has the indicated command ID.


## Syntax

 _expression_ . **DoCmd**( **_CommandID_** )

 _expression_ A variable that represents an **InvisibleApp** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
| _CommandID_|Required| **Integer**|The command to perform.|

### Return Value

nothing


## Remarks

Constants for Microsoft Visio command IDs are declared by the Visio type library in  **[VisUICmds](visuicmds-enumeration-visio.md)** and are prefixed with **visCmd** .

The  **DoCmd** method works best with commands that display dialog boxes.

For a list of commands that can be used with the  **DoCmd** method, see the topic[DoCmd/DOCMD Commands ](http://msdn.microsoft.com/library/b8390f44-607c-c32a-5200-e1559c51b2a8%28Office.15%29.aspx) in this Automation Reference.


## Example

The following macro shows how to use constants with the  **DoCmd** method. It opens a new document and displays the document stencil.


```vb
 
Public Sub DoCmd_Example() 
 
 Dim vsoDocument As Visio.Document 
 
 Set vsoDocument = Documents.Add("") 
 
 Visio.Application.DoCmd (visCmdWindowShowMasterObjects) 
 
End Sub
```


