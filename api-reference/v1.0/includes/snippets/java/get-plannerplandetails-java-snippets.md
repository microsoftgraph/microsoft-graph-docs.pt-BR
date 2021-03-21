---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a42bdcece138678326e5cdfd5d443ad84ceab171
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974802"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanDetails plannerPlanDetails = graphClient.planner().plans("{plan-id}").details()
    .buildRequest()
    .get();

```