---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 99068aa09f512553957ecdb80bdd6e725c279e9e
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015208"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPlannerPlanCollectionPage plans = graphClient.planner().plans()
    .buildRequest()
    .get();

```