---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d93e234ecfb6e5abba65312e640643dfc677feb9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477160"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests["7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee"]
    .UpdateRequest(decision,assignmentState,schedule,reason)
    .Request()
    .PostAsync();

```