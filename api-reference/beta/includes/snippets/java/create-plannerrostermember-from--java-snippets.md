---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8759320a5638d9d82ccda6cd6749c2c7fca8c94
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRosterMember plannerRosterMember = new PlannerRosterMember();
plannerRosterMember.userId = "String";

graphClient.planner().rosters("6519868f-868f-6519-8f86-19658f861965").members()
    .buildRequest()
    .post(plannerRosterMember);

```