---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d93e234ecfb6e5abba65312e640643dfc677feb9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475769"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.PrivilegedAccess["azureResources"].RoleAssignmentRequests["7c53453e-d5a4-41e0-8eb1-32d5ec8bfdee"]
    .UpdateRequest(decision,assignmentState,schedule,reason)
    .Request()
    .PostAsync();

```