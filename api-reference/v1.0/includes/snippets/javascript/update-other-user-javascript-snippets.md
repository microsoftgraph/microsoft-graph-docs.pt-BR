---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 883972a0e5ef74adbfe7a6d6f97992193f5ec90b
ms.sourcegitcommit: 3db93e28e215c0e09a65b4705ba956c6ac3b5426
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/14/2019
ms.locfileid: "36396846"
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
    .update({user : user});

```