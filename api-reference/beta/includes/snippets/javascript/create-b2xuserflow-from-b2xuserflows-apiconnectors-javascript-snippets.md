---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fb52b07551399eb2bd5a164504ea54957ea437bb4b28065fec97bd1dcfa9a502
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217192"
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
            '@odata.id': '{apiConnectorId}'
        },
        postAttributeCollection: {
            '@odata.id': '{apiConnectorId}'
        }
    }
};

await client.api('/identity/b2xUserFlows')
    .version('beta')
    .post(b2xIdentityUserFlow);

```