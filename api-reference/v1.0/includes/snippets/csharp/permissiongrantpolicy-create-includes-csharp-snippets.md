---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79f5d8d890975bb6336c5148a9e461bcc8282fff
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524120"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantConditionSet = new PermissionGrantConditionSet
{
    PermissionType = PermissionType.Delegated,
    ClientApplicationsFromVerifiedPublisherOnly = true
};

await graphClient.Policies.PermissionGrantPolicies["{id}"].Includes
    .Request()
    .AddAsync(permissionGrantConditionSet);

```