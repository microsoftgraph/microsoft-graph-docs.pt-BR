---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 65450100437c1b385b2155fc740d536c318ee3a4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35740615"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/buckets/{id}')
    .delete();

```