---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69e039f9bb212373db571577c6f63cd9c6a8b129
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452245"
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
    .update({plannerProgressTaskBoardTaskFormat : plannerProgressTaskBoardTaskFormat});

```