---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 088086278820f10df34f9a214e91240ccfb17b50
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = new PermissionGrantPolicy
{
    DisplayName = "Custom permission grant policy"
};

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"]
    .Request()
    .UpdateAsync(permissionGrantPolicy);

```