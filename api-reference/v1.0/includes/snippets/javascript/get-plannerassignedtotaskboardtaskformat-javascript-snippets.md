---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5322c160e21ba425127504fe8cd1b4c9eec71a6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35508545"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .get();

```