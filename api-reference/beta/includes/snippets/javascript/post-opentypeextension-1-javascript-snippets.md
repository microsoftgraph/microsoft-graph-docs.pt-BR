---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2a4d7978177aeccfa64de8a79e04dbbf4f65a287
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636293"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: "Annual review",
  body: {
    contentType: "HTML",
    content: "You should be proud!"
  },
  toRecipients: [
    {
      emailAddress: {
        address: "rufus@contoso.com"
      }
    }
  ],
  extensions: [
    {
      @odata.type: "microsoft.graph.openTypeExtension",
      extensionName: "Com.Contoso.Referral",
      companyName: "Wingtip Toys",
      expirationDate: "2015-12-30T11:00:00.000Z",
      dealValue: 10000
    }
  ]
};

let res = await client.api('/me/messages')
    .version('beta')
    .post(message);

```