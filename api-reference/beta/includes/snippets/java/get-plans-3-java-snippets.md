---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe264bbde5e2a8db2b8909769da14c465a1d088c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955697"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage plans = graphClient.me().planner().plans()
    .buildRequest()
    .get();

```