---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8358e029e10ee2d33dd807d79dbd969376b58057
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "35721504"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message:{  
    toRecipients:[
      {
        emailAddress: {
          address:"samanthab@contoso.onmicrosoft.com",
          name:"Samantha Booth"
        }
      },
      {
        emailAddress:{
          address:"randiw@contoso.onmicrosoft.com",
          name:"Randi Welch"
        }
      }
     ]
  },
  comment: "Samantha, Randi, would you name the group if the project is approved, please?" 
};

let res = await client.api('/me/messages/AAMkADA1MTAAAAqldOAAA=/createReply')
    .version('beta')
    .post(message);

```