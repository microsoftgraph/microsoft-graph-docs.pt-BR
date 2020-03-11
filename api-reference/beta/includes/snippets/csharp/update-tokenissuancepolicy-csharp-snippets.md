---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac98cafae299c7399c2744d4ad60cdd6a6def3d4
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591611"
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
    IsOrganizationDefault = true,
    Type = "type-value"
};

await graphClient.Policies.TokenIssuancePolicies["{id}"]
    .Request()
    .UpdateAsync(tokenIssuancePolicy);

```