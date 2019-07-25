---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2406f41f5b0ae9e6a2c93d9bbc4f97eb19a39629
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734842"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlanDetails = {
  sharedWith: {
    "6463a5ce-2119-4198-9f2a-628761df4a62" : true,
    "d95e6152-f683-4d78-9ff5-67ad180fea4a" : false,
  },
  categoryDescriptions: {
    category1: "Indoors",
    category3: null,
  }
};

let res = await client.api('/planner/plans/{plan-id}/details')
    .update({plannerPlanDetails : plannerPlanDetails});

```