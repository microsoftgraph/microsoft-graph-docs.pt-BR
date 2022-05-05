---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d246408b984fe966c570b1fe42fc20ce4048da0
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202777"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var channel = new Channel
{
    DisplayName = "My First Shared Channel",
    Description = "This is my first shared channel",
    MembershipType = ChannelMembershipType.Shared,
    Members = new ChannelMembersCollectionPage()
    {
        new AadUserConversationMember
        {
            Roles = new List<String>()
            {
                "owner"
            },
            AdditionalData = new Dictionary<string, object>()
            {
                {"user@odata.bind", "https://graph.microsoft.com/beta/users('7640023f-fe43-gv3f-9gg4-84a9efe4acd6')"}
            }
        }
    }
};

await graphClient.Teams["{team-id}"].Channels
    .Request()
    .AddAsync(channel);

```