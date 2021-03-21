---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 277c1c2d31bfbab2d76f2f47be2f6e8355d40dc9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980955"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerRoster plannerRoster = new PlannerRoster();

graphClient.planner().rosters()
    .buildRequest()
    .post(plannerRoster);

```