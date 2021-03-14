---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4654f1e10fd6d94c9013540ab2ffc3935850d087
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795929"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicy = new ClaimsMappingPolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.ServicePrincipals["{servicePrincipal-id}"].ClaimsMappingPolicies.References
    .Request()
    .AddAsync(claimsMappingPolicy);

```