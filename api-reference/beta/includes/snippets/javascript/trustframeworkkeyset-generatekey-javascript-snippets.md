---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce6e3aaf7b1801ba5463bc87bd806d09ab04927c
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37937559"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const trustFrameworkKey = {
  use: "sig",
  kty: "RSA",
  nbf: 1508969811,
  exp: 1508969811
};

let res = await client.api('/trustFramework/keySets/{id}/generateKey')
    .version('beta')
    .post(trustFrameworkKey);

```