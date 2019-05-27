---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1f1e53b6a4e8eddc6439e9ef463f8b271daa3fba
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460542"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = new Message
{
    ReceivedDateTime = "datetime-value",
    SentDateTime = "datetime-value",
    HasAttachments = true,
    Subject = "subject-value",
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    },
    BodyPreview = "bodyPreview-value"
};

await graphClient.Me.MailFolders["{id}"].Messages
    .Request()
    .AddAsync(message);

```