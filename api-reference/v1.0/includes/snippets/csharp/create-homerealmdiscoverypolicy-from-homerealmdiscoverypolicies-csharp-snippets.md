---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d18c6294df135a2d677ca81da680da923b58ff1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var homeRealmDiscoveryPolicy = new HomeRealmDiscoveryPolicy
{
    Definition = new List<String>()
    {
        "{\"HomeRealmDiscoveryPolicy\":\r\n     {\"AccelerateToFederatedDomain\":true,\r\n      \"PreferredDomain\":\"federated.example.edu\",\r\n      \"AlternateIdLogin\":{\"Enabled\":true}}}"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.HomeRealmDiscoveryPolicies
    .Request()
    .AddAsync(homeRealmDiscoveryPolicy);

```