---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43276b79e74fd3f49508691af3f03d073d370c65
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  message: {  
    isDeliveryReceiptRequested: true,
    toRecipients: [
      {
        emailAddress: {
          address: 'danas@contoso.onmicrosoft.com',
          name: 'Dana Swope'
        }
      }
     ]
  },
  comment: 'Dana, just want to make sure you get this; you\'ll need this if the project gets approved.' 
};

await client.api('/me/messages/AAMkADA1MTAAAH5JaLAAA=/createForward')
    .version('beta')
    .post(message);

```