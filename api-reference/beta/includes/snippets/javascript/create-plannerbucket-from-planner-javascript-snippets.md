---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e7189e18836bfae51e1e67144b05e365b530d60c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792214"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucket = {
  name: 'Advertising',
  planId: 'xqQg5FS2LkCp935s-FIFm2QAFkHM',
  orderHint: ' !'
};

await client.api('/planner/buckets')
    .version('beta')
    .post(plannerBucket);

```