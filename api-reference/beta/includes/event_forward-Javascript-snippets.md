---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7f546f627d75e1cc78b482b4a14d19e5394a1124
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  ToRecipients:[
      {
        emailAddress: {
          address:"danas@contoso.onmicrosoft.com",
          name:"Dana Swope"
        }
      }
     ],
  Comment: "Dana, hope you can make this meeting." 
};

let res = await client.api('/me/events/{id}/forward')
    .version('beta')
    .post(forward);

```