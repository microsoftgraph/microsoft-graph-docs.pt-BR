---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c3503ad4842cb73c18ef7c9f8b80f678be770f82
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329582"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: "Partner",
    userFlowType: "signUpOrSignIn",
    userFlowTypeVersion: 1,
    identityProviders: [
        {
            id: "Facebook-OAuth",
            type: "Facebook",
            name: "Facebook"
        }
    ]
};

let res = await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```