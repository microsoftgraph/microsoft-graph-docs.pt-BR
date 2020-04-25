---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 669826cf47f4b69894176796def8423146ca5bfa
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805488"
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