---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65b56d69416b240748289ded22a26f2c1cf2819c
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608492"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignmentRequests["7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee"]
    .Cancel()
    .Request()
    .PostAsync();

```