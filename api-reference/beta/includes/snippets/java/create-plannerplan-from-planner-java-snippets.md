---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3a5354e7ed0bb895e4d547fcabead41e1881750
ms.sourcegitcommit: 69c355eeb620b76ca70d896f984e21c32ac09eb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093566"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = new PlannerPlan();
PlannerPlanContainer container = new PlannerPlanContainer();
container.url = "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874";
plannerPlan.container = container;
plannerPlan.title = "title-value";

graphClient.planner().plans()
    .buildRequest()
    .post(plannerPlan);

```