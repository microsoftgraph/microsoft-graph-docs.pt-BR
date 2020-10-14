---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50daf78f80ab150c99c5a03f46b88f93c20aa84c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48460184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var excludes = await graphClient.Policies.PermissionGrantPolicies["microsoft-application-admin"].Excludes
    .Request()
    .GetAsync();

```