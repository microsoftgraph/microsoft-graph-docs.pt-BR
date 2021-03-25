---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82326bc31d0ad7bec24094e4ec96ba3cbe4539ad
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208717"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerPlanCollectionPage plans = graphClient.me().planner().plans()
    .buildRequest()
    .get();

```