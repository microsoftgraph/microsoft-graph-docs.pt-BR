---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7e7b059074a9d9e53e9e166ef57d0a23040782cb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800288"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: 'sig',
  kty: 'RSA',
  nbf: 1508969811,
  exp: 1508969811
};

await client.api('/trustFramework/keySets/{id}/generateKey')
    .version('beta')
    .post(trustFrameworkKey);

```