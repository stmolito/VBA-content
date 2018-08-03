---
title: RemoteItem.ConversationID Property (Outlook)
keywords: vbaol11.chm3495
f1_keywords:
- vbaol11.chm3495
ms.prod: outlook
api_name:
- Outlook.RemoteItem.ConversationID
ms.assetid: 7cef33a7-99f8-63f6-a987-6dce94fa3120
ms.date: 06/08/2017
---


# RemoteItem.ConversationID Property (Outlook)

Returns a  **String** that uniquely identifies a **[Conversation](conversation-object-outlook.md)** object that the **[RemoteItem](remoteitem-object-outlook.md)** object belongs to. Read-only.


## Syntax

 _expression_ . **ConversationID**

 _expression_ A variable that represents a **RemoteItem** object.


## Remarks

This property associates items with a conversation. These items and the conversation all have the same value in their  **ConversationID** property.

This property corresponds with the MAPI property  **PidTagConversationId** .

If the  **RemoteItem** object is created in a version of Microsoft Outlook earlier than Outlook 2013, or if Outlook is running in online mode against a version of Microsoft Exchange Server earlier than Microsoft Exchange Server 2010, this property returns the same value as the **[ConversationTopic](appointmentitem-conversationtopic-property-outlook.md)** property.


## See also


#### Concepts


[RemoteItem Object](remoteitem-object-outlook.md)

