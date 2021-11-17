---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02fb7243e8dfccdbac298bcebf425725d56280c1e7d0a00da4858ac403a07288
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
  givenName: 'Pavel',
  surname: 'Bansky',
  emailAddresses: [
    {
      address: 'pavelb@contoso.onmicrosoft.com',
      name: 'Pavel Bansky',
      type: 'personal'
    },
    {
      address: 'pavelb@fabrikam.onmicrosoft.com',
      name: 'Pavel Bansky',
      type: 'other',
      otherLabel: 'Volunteer work'
    }
  ],
  phones: [
    {
      number: '+1 732 555 0102',
      type: 'business'
    }
  ]
};

await client.api('/me/contacts')
    .version('beta')
    .post(contact);

```