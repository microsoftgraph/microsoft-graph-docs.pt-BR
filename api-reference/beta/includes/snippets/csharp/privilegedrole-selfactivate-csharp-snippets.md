---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 053da63945be69e296ea066fe0a739bd9e9ab24e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reason = "reason-value";

var duration = "duration-value";

var ticketNumber = "ticketNumber-value";

var ticketSystem = "ticketSystem-value";

await graphClient.PrivilegedRoles["{id}"]
    .SelfActivate(reason,duration,ticketNumber,ticketSystem)
    .Request()
    .PostAsync();

```