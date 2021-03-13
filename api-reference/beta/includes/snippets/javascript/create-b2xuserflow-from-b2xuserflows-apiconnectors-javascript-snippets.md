---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6308aee75bc0e6b71a703f027cafb0cf356590a2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'UserFlowWithAPIConnector',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1,
    apiConnectorConfiguration: {
        postFederationSignup: {
            '@odata.id': 'https://graph.microsoft.com/beta/identity/apiConnectors/{id}'
        },
        postAttributeCollection: {
            '@odata.id': 'https://graph.microsoft.com/beta/identity/apiConnectors/{id}'
        }
    }
};

await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```