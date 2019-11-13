---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 302cdf706e7cbb750e0f1a23cf9ea99eac776666
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302533"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancelMediaProcessingOperation = {
  all: true,
  clientContext: "clientContext-value"
};

let res = await client.api('/communications/calls/{id}/cancelMediaProcessing')
    .version('beta')
    .post(cancelMediaProcessingOperation);

```