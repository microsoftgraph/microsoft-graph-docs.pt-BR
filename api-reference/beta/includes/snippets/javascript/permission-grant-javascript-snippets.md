---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 81919889013081e2045ee6f6b8698d1fcbd49488
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: 'john@contoso.com'
    },
    {
      email: 'ryan@external.com'
    }
  ],
  roles: ['read']
};

await client.api('/shares/{encoded-sharing-url}/permission/grant')
    .version('beta')
    .post(permission);

```