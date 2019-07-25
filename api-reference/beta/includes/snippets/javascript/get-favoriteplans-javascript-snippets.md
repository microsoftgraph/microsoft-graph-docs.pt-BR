---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9599a0c0d7b015e0f6c5c8399b60f0b2ff72a894
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720399"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/favoritePlans')
    .version('beta')
    .get();

```