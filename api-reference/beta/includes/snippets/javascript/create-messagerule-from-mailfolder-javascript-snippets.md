---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9f2ce079fd021b2e8a52a3f0a91b1070b5a46f9a97c3451544e9a1d18bdf74f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899951"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const messageRule = {
    displayName: 'From partner',      
    sequence: 2,      
    isEnabled: true,          
    conditions: {
        senderContains: [
          'adele'       
        ]
     },
     actions: {
        forwardTo: [
          {
             emailAddress: {
                name: 'Alex Wilbur',
                address: 'AlexW@contoso.onmicrosoft.com'
              }
           }
        ],
        stopProcessingRules: true
     }    
};

await client.api('/me/mailFolders/inbox/messagerules')
    .version('beta')
    .post(messageRule);

```