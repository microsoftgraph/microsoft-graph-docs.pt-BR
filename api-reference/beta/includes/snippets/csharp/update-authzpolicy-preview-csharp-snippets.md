---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb87dcfb829ed92f14ea83cc712ee38e59e5b317
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791338"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    EnabledPreviewFeatures = new List<String>()
    {
        "assignGroupsToRoles"
    }
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```