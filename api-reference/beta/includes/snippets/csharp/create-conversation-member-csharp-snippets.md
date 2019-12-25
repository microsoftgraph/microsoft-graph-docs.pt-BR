---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b56887b5e7d47260b3906cad36af3a904b49488
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868735"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"user@odata.bind","https://graph.microsoft.com/beta/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"}
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Members
    .Request()
    .AddAsync(conversationMember);

```