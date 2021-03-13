---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 167ce3fc827274e7d1cb2c85ffd9fa98af659798
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805356"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat')
    .version('beta')
    .update(plannerBucketTaskBoardTaskFormat);

```