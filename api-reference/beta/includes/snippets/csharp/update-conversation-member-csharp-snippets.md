---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8843c7561b7e5696b419e9a9154f3928d82f195f0f0eb20d0b33ade40bfafc8e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326670"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conversationMember = new AadUserConversationMember
{
    Roles = new List<String>()
    {
        "owner"
    }
};

await graphClient.Teams["{team-id}"].Channels["{channel-id}"].Members["{conversationMember-id}"]
    .Request()
    .UpdateAsync(conversationMember);

```