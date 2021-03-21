---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f30d0c822b4491c36820e280d083a5e27bb9d8d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982498"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UUID servicePlanId = UUID.fromString("28f42d6f-8034-4a0f-9d8a-a218a63b3299");

UUID skuId = UUID.fromString("465a2a90-5e59-456d-a7b8-127b9fb2e484");

graphClient.me()
    .activateServicePlan(UserActivateServicePlanParameterSet
        .newBuilder()
        .withServicePlanId(servicePlanId)
        .withSkuId(skuId)
        .build())
    .buildRequest()
    .post();

```