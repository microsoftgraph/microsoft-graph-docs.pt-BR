---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e0b060af7020095e156f1e5a9ac1a9f145f76d64
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636376"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .update(plannerProgressTaskBoardTaskFormat);

```