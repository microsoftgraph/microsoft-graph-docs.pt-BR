---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 62a1ffcf76c25cb4d1e35c46f3b721706fd52855
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589773"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activityBasedTimeoutPolicy = new ActivityBasedTimeoutPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.ActivityBasedTimeoutPolicies["{id}"]
    .Request()
    .UpdateAsync(activityBasedTimeoutPolicy);

```