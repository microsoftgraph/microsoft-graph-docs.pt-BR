---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45770eb3b019c0a0f8e58f4be35486c53f6dcae1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785764"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/planner/buckets/{id}')
    .delete();

```