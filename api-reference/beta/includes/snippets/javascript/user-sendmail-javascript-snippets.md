---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f8be9a91acf94e71e924316eb1ad4d445b74891
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48604596"
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
          address: "samanthab@contoso.onmicrosoft.com"
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
    .version('beta')
    .post(sendMail);

```