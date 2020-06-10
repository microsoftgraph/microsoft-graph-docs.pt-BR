---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 930887864a037a3eeee7c9e945b88ae6a437e934
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681932"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var team = new Team
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"template@odata.bind", "https://graph.microsoft.com/beta/teamsTemplates('standard')"},
        {"group@odata.bind", "https://graph.microsoft.com/v1.0/groups('groupId')"}
    }
};

await graphClient.Teams
    .Request()
    .AddAsync(team);

```