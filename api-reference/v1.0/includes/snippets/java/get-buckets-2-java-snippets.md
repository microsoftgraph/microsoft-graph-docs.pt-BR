---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f29d567d90c48f3e900878e8c60ba86541502143
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210846"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerBucketCollectionPage buckets = graphClient.planner().plans("{plan-id}").buckets()
    .buildRequest()
    .get();

```