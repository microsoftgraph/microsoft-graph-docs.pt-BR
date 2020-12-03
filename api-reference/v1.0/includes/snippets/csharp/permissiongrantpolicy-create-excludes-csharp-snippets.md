---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ac13d1c44ecc9918633e211ddeb32d126a37eeb
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524189"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ResourceApplication = "00000003-0000-0000-c000-000000000000"
};

await graphClient.Policies.PermissionGrantPolicies["my-custom-consent-policy"].Excludes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```