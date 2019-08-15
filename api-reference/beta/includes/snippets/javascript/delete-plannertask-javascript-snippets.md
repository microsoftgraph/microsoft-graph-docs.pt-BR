---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f14b1115e9a430438fa617649e3eeb7dcd6afcaf
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413110"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{id}')
    .version('beta')
    .delete();

```