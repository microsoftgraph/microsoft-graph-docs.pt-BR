---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97486d3d3974d6b385f1f887278ec702f5985423
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789580"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.PermissionGrantPolicies["{permissionGrantPolicy-id}"].Excludes["{permissionGrantConditionSet-id}"]
    .Request()
    .DeleteAsync();

```