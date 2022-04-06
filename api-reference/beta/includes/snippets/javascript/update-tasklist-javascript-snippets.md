---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 606129793372e0303226a9c2f6b09d436ea25471
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528005"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const baseTaskList = {
    '@odata.type': '#microsoft.graph.taskList',
    displayName: 'Travel Plan'
};

await client.api('/me/tasks/lists/AAMkAGVjMzJmMWZjLTgyYjgtNGIyNi1hOGQ0LWRjMjNmMGRmOWNiYQAuAAAAAAAboFs')
    .version('beta')
    .update(baseTaskList);

```