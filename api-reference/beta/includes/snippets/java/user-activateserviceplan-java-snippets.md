---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 764f1b812d9291e00e8a4d60a68234a1e5f36fce
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775035"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID servicePlanId = UUID.fromString("28f42d6f-8034-4a0f-9d8a-a218a63b3299");

UUID skuId = UUID.fromString("465a2a90-5e59-456d-a7b8-127b9fb2e484");

graphClient.me()
    .activateServicePlan(servicePlanId,skuId)
    .buildRequest()
    .post();

```