---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9bd9468060d310720c588381c312cc9c6d6d39d9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const user = {
  accountEnabled: true,
  businessPhones: [
    "businessPhones-value"
  ],
  city: "city-value"
};

let res = await client.api('/me')
    .update({user : user});

```