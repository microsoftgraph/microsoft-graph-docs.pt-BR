---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64d2372ecc68f849d7c7c8608ce347726ace193be61dbe97559ce6ea6bfafafb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326998"
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

await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleSettings["{governanceRoleSetting-id}"]
    .Request()
    .UpdateAsync(governanceRoleSetting);

```