---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 443cc2319e01fdeb46fc321d6bd2eb6068d42ebc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34481076"
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