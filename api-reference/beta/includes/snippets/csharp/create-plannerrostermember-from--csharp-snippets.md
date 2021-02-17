---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a280e8e6a426e0fbab5574c4e03c40212d8c57d8
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272422"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerRosterMember = new PlannerRosterMember
{
    UserId = "String"
};

await graphClient.Planner.Rosters["6519868f-868f-6519-8f86-19658f861965"].Members
    .Request()
    .AddAsync(plannerRosterMember);

```