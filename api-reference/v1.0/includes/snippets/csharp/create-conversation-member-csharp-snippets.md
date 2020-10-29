---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d46b61eaba1c682bfa18ec8735f58fbb73e62115
ms.sourcegitcommit: 60ced1be6ed8dd2d23263090a1cfbc16689bb043
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48782895"
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
        {"user@odata.bind", "https://graph.microsoft.com/v1.0/users/8b081ef6-4792-4def-b2c9-c363a1bf41d5"}
    }
};

await graphClient.Teams["{id}"].Channels["{id}"].Members
    .Request()
    .AddAsync(conversationMember);

```