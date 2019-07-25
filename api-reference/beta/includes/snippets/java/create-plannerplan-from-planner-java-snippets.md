---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 463307cacf6d48d9622667cea7b7bbf95c01aed9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876656"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlan plannerPlan = new PlannerPlan();
plannerPlan.owner = "ebf3b108-5234-4e22-b93d-656d7dae5874";
plannerPlan.title = "title-value";

graphClient.planner().plans()
    .buildRequest()
    .post(plannerPlan);

```