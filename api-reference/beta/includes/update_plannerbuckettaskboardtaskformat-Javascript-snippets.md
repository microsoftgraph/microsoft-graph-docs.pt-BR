---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70788378a3c2a92d363341901c3171262bcba906
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/hsOf2dhOJkqyYYZEtdzDe2QAIUCR/bucketTaskBoardFormat')
    .version('beta')
    .update({plannerBucketTaskBoardTaskFormat : plannerBucketTaskBoardTaskFormat});

```