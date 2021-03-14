---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47b35f688905842a8a6e06999e5ed0d08a0b61c7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tasks = await client.api('/planner/buckets/{bucket-id}/tasks')
    .get();

```