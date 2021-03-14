---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab402239c238b0250e67a4680e4405646c070832
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/tasks')
    .get();

```