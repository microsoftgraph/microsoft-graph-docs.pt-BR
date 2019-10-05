---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7c3b08e01c8d4ccf910aa2d1e42ae531b41266a
ms.sourcegitcommit: 46ee19b244349e2a1537f0c44c576d7c01cf03a9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2019
ms.locfileid: "37402345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = new GovernanceRoleSetting
{
    AdminEligibleSettings = new List<GovernanceRuleSetting>()
    {
        new GovernanceRuleSetting
        {
            RuleIdentifier = "ExpirationRule",
            Setting = "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
        }
    }
};

await graphClient.PrivilegedAccess["azureResources"].RoleSettings["5fb5aef8-1081-4b8e-bb16-9d5d0385bab5"]
    .Request()
    .UpdateAsync(governanceRoleSetting);

```