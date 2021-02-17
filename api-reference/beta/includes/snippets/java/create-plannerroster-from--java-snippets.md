---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab942dbe71f82c5d54e223aa9eee80bb4bcd60fd
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272000"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = new PlannerRoster();

graphClient.planner().rosters()
    .buildRequest()
    .post(plannerRoster);

```