---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 80492e83264120091482df6029cdbb0f8bd8b40f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443128"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoleAssignments["{id}"]
    .MakePermanent(reason,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```