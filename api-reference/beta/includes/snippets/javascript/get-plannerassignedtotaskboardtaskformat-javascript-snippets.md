---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bf934f131ddd37dbbf0490c88d8e6408ee5f600a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622538"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh/assignedToTaskBoardFormat')
    .version('beta')
    .get();

```