---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8ee1bf38c21891d788874e760c3c892c76ea28d2
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556240"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  businessPhones: [
    "+1 425 555 0109"
  ],
  officeLocation: "18/2111"
};

let res = await client.api('/me')
    .version('beta')
    .update(user);

```