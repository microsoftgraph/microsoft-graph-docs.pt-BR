---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8ad3e2bafc68239db0f81c7f0972b4da1e6406c
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51572993"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var topic = new TeamworkActivityTopic
{
    Source = TeamworkActivityTopicSource.EntityUrl,
    Value = "https://graph.microsoft.com/beta/chats/{chatId}/messages/{messageId}"
};

var activityType = "approvalRequired";

var previewText = new ItemBody
{
    Content = "Deployment requires your approval"
};

var recipient = new AadUserNotificationRecipient
{
    UserId = "569363e2-4e49-4661-87f2-16f245c5d66a"
};

var templateParameters = new List<KeyValuePair>()
{
    new KeyValuePair
    {
        Name = "approvalTaskId",
        Value = "2020AAGGTAPP"
    }
};

await graphClient.Chats["{chat-id}"]
    .SendActivityNotification(topic,activityType,null,previewText,templateParameters,recipient)
    .Request()
    .PostAsync();

```