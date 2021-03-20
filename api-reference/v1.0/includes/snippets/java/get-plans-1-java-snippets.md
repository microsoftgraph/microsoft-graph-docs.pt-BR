---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99068aa09f512553957ecdb80bdd6e725c279e9e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941504"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage plans = graphClient.planner().plans()
    .buildRequest()
    .get();

```