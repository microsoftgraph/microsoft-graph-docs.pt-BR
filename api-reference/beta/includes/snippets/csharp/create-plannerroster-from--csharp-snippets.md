---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4b214c1477ca54764ac32523576aa420f928ca4
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRoster = new PlannerRoster
{
};

await graphClient.Planner.Rosters
    .Request()
    .AddAsync(plannerRoster);

```