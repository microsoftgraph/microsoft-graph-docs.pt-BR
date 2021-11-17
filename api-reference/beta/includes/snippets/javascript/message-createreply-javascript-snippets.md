---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35b878921c1cbf4b50b3bcb04048931b688c43df0937668b7d396d8191f81b51
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message: {  
    toRecipients: [
      {
        emailAddress: {
          address: 'samanthab@contoso.onmicrosoft.com',
          name: 'Samantha Booth'
        }
      },
      {
        emailAddress: {
          address: 'randiw@contoso.onmicrosoft.com',
          name: 'Randi Welch'
        }
      }
     ]
  },
  comment: 'Samantha, Randi, would you name the group if the project is approved, please?' 
};

await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply')
    .version('beta')
    .post(message);

```