---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2576cef01086e7acc67911ef5d42495412d14093
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61006709"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
topic := msgraphsdk.NewTeamworkActivityTopic()
requestBody.SetTopic(topic)
source := "entityUrl"
topic.SetSource(&source)
value := "https://graph.microsoft.com/v1.0/chats/{chatId}/messages/{messageId}"
topic.SetValue(&value)
activityType := "approvalRequired"
requestBody.SetActivityType(&activityType)
previewText := msgraphsdk.NewItemBody()
requestBody.SetPreviewText(previewText)
content := "Deployment requires your approval"
previewText.SetContent(&content)
recipient := msgraphsdk.NewTeamworkNotificationRecipient()
requestBody.SetRecipient(recipient)
recipient.SetAdditionalData(map[string]interface{}{
    "@odata.type": "Microsoft.Teams.GraphSvc.aadUserNotificationRecipient",
    "userId": "jacob@contoso.com",
}
requestBody.SetTemplateParameters( []KeyValuePair {
    msgraphsdk.NewKeyValuePair(),
    SetAdditionalData(map[string]interface{}{
        "name": "approvalTaskId",
        "value": "2020AAGGTAPP",
    }
}
options := &msgraphsdk.SendActivityNotificationRequestBuilderPostOptions{
    Body: requestBody,
}
chatId := "chat-id"
graphClient.ChatsById(&chatId).SendActivityNotification().Post(options)


```