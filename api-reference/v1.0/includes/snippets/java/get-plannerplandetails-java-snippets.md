---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c69b21d6926972a493f106dd4cecfc925e1ccaf8
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35888788"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("{plan-id}").details()
    .buildRequest()
    .get();

```