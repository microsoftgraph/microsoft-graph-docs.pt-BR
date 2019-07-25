---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ea14947f3c2f7b1b5341ea2dff4988fac872521e
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35876354"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("xqQg5FS2LkCp935s-FIFm2QAFkHM").details()
    .buildRequest()
    .get();

```