---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 176270527a6dc1265dc28985537d0c30e628cca6
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460220"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var permissionGrantPolicy = await graphClient.Policies.PermissionGrantPolicies["microsoft-user-default-low"]
    .Request()
    .GetAsync();

```