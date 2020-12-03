---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5784883d01639b6b3703188464956cdec3a3146
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "49556300"
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

let res = await client.api('/users/{id}')
    .update(user);

```