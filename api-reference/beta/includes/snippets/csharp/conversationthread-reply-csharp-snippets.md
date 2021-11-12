---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8029f5dbcd996c33ccb4595f9f4cc7e55330f257baec65fb46fb2f814d444c3c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156506"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var post = new Post
{
    Body = new ItemBody
    {
        ContentType = BodyType.Text,
        Content = "content-value"
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"]
    .Reply(post)
    .Request()
    .PostAsync();

```