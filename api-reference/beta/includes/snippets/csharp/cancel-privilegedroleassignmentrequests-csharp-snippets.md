---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65b56d69416b240748289ded22a26f2c1cf2819c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498668"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedRoleAssignmentRequests["7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee"]
    .Cancel()
    .Request()
    .PostAsync();

```