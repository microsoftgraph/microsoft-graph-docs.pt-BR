---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef871a1fadc96648d89c0c0856c7cdcde582c9b1
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707624"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chatMessage = new ChatMessage
{
    Body = new ItemBody
    {
        Content = "Hello world"
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Messages["{id}"].Replies
    .Request()
    .AddAsync(chatMessage);

```