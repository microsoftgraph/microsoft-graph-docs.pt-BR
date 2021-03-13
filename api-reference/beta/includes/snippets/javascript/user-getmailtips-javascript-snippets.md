---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e7762f2ff1896a3e2b4e489ca3102137816e4ae
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799844"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailTips = {
    EmailAddresses: [
        'danas@contoso.onmicrosoft.com', 
        'fannyd@contoso.onmicrosoft.com'
    ],
    MailTipsOptions: 'automaticReplies, mailboxFullStatus'
};

await client.api('/me/getMailTips')
    .version('beta')
    .post(mailTips);

```