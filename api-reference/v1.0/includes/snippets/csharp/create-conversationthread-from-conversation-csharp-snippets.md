---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 758b7015bd3eb43277894d31b65414141fb2a4b5
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945690"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationThread = new ConversationThread
{
    Topic = "topic-value",
    Posts = new ConversationThreadPostsCollectionPage()
    {
        new Post
        {
            Body = new ItemBody
            {
                ContentType = BodyType.Html,
                Content = "this is body content"
            }
        }
    }
};

await graphClient.Groups["{id}"].Conversations["{id}"].Threads
    .Request()
    .AddAsync(conversationThread);

```