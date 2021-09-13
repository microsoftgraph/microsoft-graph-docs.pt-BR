---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15462f48deebf2254af301967ab6285b02a54ff6fc03376ebe77c1abc8a4b4ba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56900048"
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
      address: 'pavelb@fabrikam.onmicrosoft.com',
      name: 'Pavel Bansky'
    }
  ],
  businessPhones: [
    '+1 732 555 0102'
  ]
};

await client.api('/me/contacts')
    .post(contact);

```