---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae7a61ca6fd0414172340c49a812f443d943300d
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556171"
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
    .update(user);

```