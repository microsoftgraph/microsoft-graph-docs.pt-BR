---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5983ea869e9913919343778cc41524fb2312f1e3
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636380"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerBucketTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/{task-id}/bucketTaskBoardFormat')
    .update(plannerBucketTaskBoardTaskFormat);

```