---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eca99f74caea04bb913e515db51fe0b4371b2421
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498704"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: "A6673H Ejkl!"
};

let res = await client.api('/planner/tasks/'id'/progressTaskBoardFormat')
    .version('beta')
    .update({plannerProgressTaskBoardTaskFormat : plannerProgressTaskBoardTaskFormat});

```