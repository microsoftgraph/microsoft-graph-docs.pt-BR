---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9505222d638055aa4e4ec5fbc6c52a97afdecbd8
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609657"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}')
    .get();

```