---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 988f23fdbf5df753773d021bad7b9af5e5a12c9f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35507447"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const sendMail = {
  message: {
    subject: "Meet for lunch?",
    body: {
      contentType: "Text",
      content: "The new cafeteria is open."
    },
    toRecipients: [
      {
        emailAddress: {
          address: "fannyd@contoso.onmicrosoft.com"
        }
      }
    ],
    ccRecipients: [
      {
        emailAddress: {
          address: "danas@contoso.onmicrosoft.com"
        }
      }
    ]
  },
  saveToSentItems: "false"
};

let res = await client.api('/me/sendMail')
    .post(sendMail);

```