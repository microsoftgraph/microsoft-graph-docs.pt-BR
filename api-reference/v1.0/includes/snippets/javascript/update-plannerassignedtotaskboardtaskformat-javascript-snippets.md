---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2f95449538ac52a0b3a7b27fda2d80679cb3a4a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791674"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerAssignedToTaskBoardTaskFormat = {
  orderHintsByAssignee: {
    'aaa27244-1db4-476a-a5cb-004607466324': '8566473P 957764Jk!'
  }
};

await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .update(plannerAssignedToTaskBoardTaskFormat);

```