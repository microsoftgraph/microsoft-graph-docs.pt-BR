---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4169ce624b9823da7e1c50c20473dcfd31d868ebca2966ec9de3b56ae651e98a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216433"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenLifetimePolicy = new TokenLifetimePolicy
{
    Definition = new List<String>()
    {
        "definition-value"
    },
    DisplayName = "displayName-value",
    IsOrganizationDefault = true
};

await graphClient.Policies.TokenLifetimePolicies["{tokenLifetimePolicy-id}"]
    .Request()
    .UpdateAsync(tokenLifetimePolicy);

```