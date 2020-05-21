---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c87df357a1dc6111ffd762fab88dee6e7750ad66
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333157"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const removeKey = {
    keyId: "f0b0b335-1d71-4883-8f98-567911bfdca6",
    proof:"eyJ0eXAiOiJ..."
};

let res = await client.api('/applications/{id}/removeKey')
    .version('beta')
    .post(removeKey);

```