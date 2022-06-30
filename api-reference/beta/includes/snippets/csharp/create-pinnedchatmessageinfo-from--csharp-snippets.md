---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8dbdf272988f174134961e6dec6da3026c5c495d
ms.sourcegitcommit: 54ba08a80db85b9e84813387e8c4416eca44fa8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2022
ms.locfileid: "65693858"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pinnedChatMessageInfo = new PinnedChatMessageInfo
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"message@odata.bind", "https://graph.microsoft.com/beta/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages/1616964509832"}
    }
};

await graphClient.Chats["{chat-id}"].PinnedMessages
    .Request()
    .AddAsync(pinnedChatMessageInfo);

```