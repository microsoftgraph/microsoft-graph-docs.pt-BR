---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66a27858136faa233bddba7d25ebf4b2c30cde623291b54f5137b1b638edaa4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275492"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerProgressTaskBoardTaskFormat = {
  orderHint: 'A6673H Ejkl!'
};

await client.api('/planner/tasks/{task-id}/progressTaskBoardFormat')
    .update(plannerProgressTaskBoardTaskFormat);

```