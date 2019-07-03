---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5e14eb8b568b26fb1a931d86bc40fd340358fe3c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476782"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const mailTips = {
    EmailAddresses: [
        "danas@contoso.onmicrosoft.com", 
        "fannyd@contoso.onmicrosoft.com"
    ],
    MailTipsOptions: "automaticReplies, mailboxFullStatus"
};

let res = await client.api('/me/getMailTips')
    .version('beta')
    .post(mailTips);

```