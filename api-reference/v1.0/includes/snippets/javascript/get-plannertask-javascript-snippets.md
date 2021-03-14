---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17c6db5be8b59f58528c82a77c4c4c41431a7d78
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786959"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerTask = await client.api('/planner/tasks/{task-id}')
    .get();

```