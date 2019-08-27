---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0413da264910c1b6cd46bfbd1180757946d9451
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636260"
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

let res = await client.api('/servicePrincipals/{id}/owners')
    .version('beta')
    .post(directoryObject);

```