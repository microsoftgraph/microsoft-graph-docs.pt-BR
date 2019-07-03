---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9505222d638055aa4e4ec5fbc6c52a97afdecbd8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}')
    .get();

```