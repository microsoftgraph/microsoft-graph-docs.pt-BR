---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe2e94f1e9bcfc56060bdbbe9ce4befe97c8fdff
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453576"
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

let res = await client.api('/applications/{id}/owners')
    .version('beta')
    .post({directoryObject : directoryObject});

```