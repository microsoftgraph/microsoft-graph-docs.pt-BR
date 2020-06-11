---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5093f32ef3ca4741c094819d46172d803473ec2c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683998"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.id", "https://graph.microsoft.com/v1.0/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"}
    }
};

await graphClient.Applications["{id}"].TokenIssuancePolicies.References
    .Request()
    .AddAsync(tokenIssuancePolicy);

```