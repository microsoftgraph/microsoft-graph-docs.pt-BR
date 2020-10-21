---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5322c160e21ba425127504fe8cd1b4c9eec71a6
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48611613"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/tasks/{task-id}/assignedToTaskBoardFormat')
    .get();

```