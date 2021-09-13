---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71442701558ebdc0a82d1814b852b56da0a3f744abb995792e4d28f5a18d7e24
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100676"
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