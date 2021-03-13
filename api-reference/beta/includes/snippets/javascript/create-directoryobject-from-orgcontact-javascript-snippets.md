---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40b1fb66213fc4d4bfa02bdc3c9cddc064a01219
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787409"
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

await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .post(directoryObject);

```