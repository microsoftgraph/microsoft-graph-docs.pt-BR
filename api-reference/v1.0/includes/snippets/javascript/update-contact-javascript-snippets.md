---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9efcd6bb1c1b40ffb7c3ce6eebf8d196ba0d6a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  homeAddress: {
    street: '123 Some street',
    city: 'Seattle',
    state: 'WA',
    postalCode: '98121'
  },
  birthday: '1974-07-22'
};

await client.api('/me/contacts/{id}')
    .update(contact);

```