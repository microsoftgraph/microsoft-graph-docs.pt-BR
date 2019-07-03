---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 443cc2319e01fdeb46fc321d6bd2eb6068d42ebc
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  directoryObject: {
  }
};

let res = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post({directoryObject : directoryObject});

```