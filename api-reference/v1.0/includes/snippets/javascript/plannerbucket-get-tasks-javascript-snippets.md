---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31288720573c8e937ba067a5152fb3d6994c3b9a
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37637856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{task-id}/tasks')
    .get();

```