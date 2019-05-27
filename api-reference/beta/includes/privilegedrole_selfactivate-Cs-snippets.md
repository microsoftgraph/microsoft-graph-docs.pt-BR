---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 053da63945be69e296ea066fe0a739bd9e9ab24e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443219"
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