---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4a6e48b3421a0aea3eb25b1721183ba24d2f2c6
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272294"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionWithReferencesPage rosterPlans = graphClient.users("{usersId}").planner().rosterPlans()
    .buildRequest()
    .get();

```