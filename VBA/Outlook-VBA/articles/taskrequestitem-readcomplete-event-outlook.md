---
title: TaskRequestItem.ReadComplete Event (Outlook)
ms.assetid: 2f92c2d2-742c-42b0-47c3-b9694169d8db
ms.date: 06/08/2017
ms.prod: outlook
---


# TaskRequestItem.ReadComplete Event (Outlook)
Occurs when Outlook has completed reading the properties of the item.

## Version information

Version Added: Outlook 2013 


## Syntax

 _expression_ . **ReadComplete**_(Cancel)_

 _expression_ A variable that represents a **TaskRequestItem** object.


### Parameters



|**Name**|**Required/Optional**|**Data type**|**Description**|
|:-----|:-----|:-----|:-----|
|||||
| _Cancel_|Required| **Boolean**|(Not used in VBScript).  **False** when the event occurs. If the event procedure sets this argument to **True**, the read operation is not completed and the item is not displayed in the Reading Pane or inspector.|

## Remarks

The  **ReadComplete** event occurs after the[BeforeRead](taskrequestitem-beforeread-event-outlook.md) event and before the[Read](taskrequestitem-read-event-outlook.md) event for the item.

To determine when the item is unloaded from memory, use the [Unload](taskrequestitem-unload-event-outlook.md) event.

The  **ReadComplete** event corresponds to the Exchange Client Extensions (ECE) event **IExchExtMessageEvents::OnReadComplete**.


## See also


#### Concepts


[TaskRequestItem Object](taskrequestitem-object-outlook.md)

