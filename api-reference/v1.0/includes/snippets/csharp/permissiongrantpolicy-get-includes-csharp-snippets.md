---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e87c3ce8df7e01b4a1b015c0d48fd1e019ce0cd2
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49524309"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var includes = await graphClient.Policies.PermissionGrantPolicies["microsoft-application-admin"].Includes
    .Request()
    .GetAsync();

```