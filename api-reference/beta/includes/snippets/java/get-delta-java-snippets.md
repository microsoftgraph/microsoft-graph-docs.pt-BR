---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: edccc22c11f458b745e710c7063750d1ac75463e
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50972189"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PlannerDeltaDeltaCollectionPage delta = graphClient.me().planner().all()
    .delta()
    .buildRequest()
    .get();

```