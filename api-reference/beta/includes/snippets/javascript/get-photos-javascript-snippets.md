---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8443f1d294d01cb7fa7f9e742007534858d23f3
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711958"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .version('beta')
    .get();

```