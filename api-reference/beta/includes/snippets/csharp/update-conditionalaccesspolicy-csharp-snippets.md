---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c5a76aecc3553d2c625a1071f14a861079164c1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936706"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicy = new ConditionalAccessPolicy
{
    Conditions = new ConditionalAccessConditionSet
    {
        SignInRiskLevels = new List<RiskLevel>()
        {
            RiskLevel.High,
            RiskLevel.Medium,
            RiskLevel.Low
        }
    }
};

await graphClient.ConditionalAccess.Policies["{id}"]
    .Request()
    .UpdateAsync(conditionalAccessPolicy);

```