---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c5afb922674d49e69009b54457f64678ecb22ff
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788684"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const forward = {
  comment: 'comment-value',
  toRecipients: [
    {
      emailAddress: {
        name: 'name-value',
        address: 'address-value'
      }
    }
  ]
};

await client.api('/me/messages/{id}/forward')
    .post(forward);

```