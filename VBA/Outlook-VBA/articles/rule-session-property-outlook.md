---
title: Rule.Session Property (Outlook)
keywords: vbaol11.chm2166
f1_keywords:
- vbaol11.chm2166
ms.prod: outlook
api_name:
- Outlook.Rule.Session
ms.assetid: 7502f919-cf8f-d795-87b1-9812c0d150d1
ms.date: 06/08/2017
---


# Rule.Session Property (Outlook)

Returns the  **[NameSpace](namespace-object-outlook.md)** object for the current session. Read-only.


## Syntax

 _expression_ . **Session**

 _expression_ A variable that represents a **Rule** object.


## Remarks

The  **Session** property and the **[GetNamespace](application-getnamespace-method-outlook.md)** method can be used interchangeably to obtain the **NameSpace** object for the current session. Both members serve the same purpose. For example, the following statements perform the same function:


```vb
Set objNamespace = Application.GetNamespace("MAPI") 
```


```vb
Set objSession = Application.Session
```


## See also


#### Concepts


[Rule Object](rule-object-outlook.md)

