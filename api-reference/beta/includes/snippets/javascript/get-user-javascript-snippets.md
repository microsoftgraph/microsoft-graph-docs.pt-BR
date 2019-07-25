---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b576a2f53f1dab69a4518c87a9e41cfcf52085a9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714285"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me')
    .version('beta')
    .get();

```