---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 176270527a6dc1265dc28985537d0c30e628cca6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524476"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = await graphClient.Policies.PermissionGrantPolicies["microsoft-user-default-low"]
    .Request()
    .GetAsync();

```