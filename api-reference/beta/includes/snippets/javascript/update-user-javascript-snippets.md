---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 668cfae6047c2e974eafdcc107c89d859a2d648f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    '+1 425 555 0109'
  ],
  officeLocation: '18/2111'
};

await client.api('/me')
    .version('beta')
    .update(user);

```