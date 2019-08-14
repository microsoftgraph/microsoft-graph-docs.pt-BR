---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8afe55a1b036fc71a6c80a28f44ecbe724f7b2e
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396902"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    "businessPhones-value"
  ],
  officeLocation: "city-value"
};

let res = await client.api('/users/{id}')
    .version('beta')
    .update({user : user});

```