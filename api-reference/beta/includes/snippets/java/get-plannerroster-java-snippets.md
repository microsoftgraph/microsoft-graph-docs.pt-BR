---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 810bdee5cec7f89dd6317d1fb017b9d21ae122ef
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271883"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965")
    .buildRequest()
    .get();

```