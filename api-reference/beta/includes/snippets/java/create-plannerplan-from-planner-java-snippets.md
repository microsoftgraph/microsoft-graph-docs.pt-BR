---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 886ad52480e0b32ccf51fdce1e99a845ac0d8ee35ce460a579900fd074f59ba2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158752"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = new PlannerPlan();
PlannerPlanContainer container = new PlannerPlanContainer();
container.url = "https://graph.microsoft.com/beta/groups/ebf3b108-5234-4e22-b93d-656d7dae5874";
plannerPlan.container = container;
plannerPlan.title = "title-value";

graphClient.planner().plans()
    .buildRequest()
    .post(plannerPlan);

```