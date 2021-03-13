---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab37f3f59259dc59282c2b4dcbdf855e4035e319
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787301"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var privilegedRoleSettings = await graphClient.PrivilegedRoles["{privilegedRole-id}"].Settings
    .Request()
    .GetAsync();

```