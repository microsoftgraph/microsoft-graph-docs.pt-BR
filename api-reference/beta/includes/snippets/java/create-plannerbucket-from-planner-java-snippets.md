---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3cea7801654e7384091ad8ca885ccca1ae9ee499596af5104de005812d61827d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326828"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucket plannerBucket = new PlannerBucket();
plannerBucket.name = "Advertising";
plannerBucket.planId = "xqQg5FS2LkCp935s-FIFm2QAFkHM";
plannerBucket.orderHint = " !";

graphClient.planner().buckets()
    .buildRequest()
    .post(plannerBucket);

```