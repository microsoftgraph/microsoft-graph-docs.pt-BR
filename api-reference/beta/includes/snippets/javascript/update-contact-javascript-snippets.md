---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a4654867f0ac67f39ce79990a930b1659f45a7
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/21/2019
ms.locfileid: "36636126"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const contact = {
    emailAddresses:[
        {
            type:"personal",
            name:"Pavel Bansky",
            address:"pavelb@adatum.onmicrosoft.com"
        },
        {
          address: "pavelb@fabrikam.onmicrosoft.com",
          name: "Pavel Bansky",
          type: "other",
          otherLabel: "Volunteer work"
        }
    ]
};

let res = await client.api('/me/contacts/AAMkADh6v5AAAvgTCEAAA=')
    .version('beta')
    .update(contact);

```