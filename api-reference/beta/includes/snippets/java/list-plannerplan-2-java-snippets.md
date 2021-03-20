---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4a6e48b3421a0aea3eb25b1721183ba24d2f2c6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953214"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionWithReferencesPage rosterPlans = graphClient.users("{usersId}").planner().rosterPlans()
    .buildRequest()
    .get();

```