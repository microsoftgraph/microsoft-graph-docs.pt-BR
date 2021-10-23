---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0e6e62b9cbf9c5e75952e23d497855a2922eb061fb94031ced7c818a95dcc97
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var chat = new Chat
{
    ChatType = ChatType.OneOnOne,
    Members = new ChatMembersCollectionPage()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"}
            }
        },
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('82af01c5-f7cc-4a2e-a728-3a5df21afd9d')"}
            }
        }
    }
};

await graphClient.Chats
    .Request()
    .AddAsync(chat);

```