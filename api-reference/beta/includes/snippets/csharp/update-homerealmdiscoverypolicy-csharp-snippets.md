---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 669826cf47f4b69894176796def8423146ca5bfa
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590034"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.HomeRealmDiscoveryPolicies["{id}"]
    .Request()
    .UpdateAsync(homeRealmDiscoveryPolicy);

```