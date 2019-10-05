---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 54deaaf5fa0eb3193e26a7653855f813c7637008
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402270"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","#Microsoft.Teams.Core.channel"}
    },
    MembershipType = ChannelMembershipType.Private,
    DisplayName = "My First Private Channel",
    Description = "This is my first private channels",
    Members = new List<ConversationMember>()
    {
        new ConversationMember
        {
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind","https://graph.microsoft.com/beta/users('{user_id}')"},
                {"@odata.type","#microsoft.graph.aadUserConversationMember"}
            },
            Roles = new List<String>()
            {
                "owner"
            }
        }
    }
};

await graphClient.Teams["{group_id}"].Channels
    .Request()
    .AddAsync(channel);

```