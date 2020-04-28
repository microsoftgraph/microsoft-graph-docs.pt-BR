---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e45ba4ab70e51a766e0a12f32a4075d9ef047cf2
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805350"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = new TokenIssuancePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenIssuancePolicies
    .Request()
    .AddAsync(tokenIssuancePolicy);

```