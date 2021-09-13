---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 970b8813116c57dbd90e918f5e108e185687030a50c850cdaa757521af813137
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216487"
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
            '@odata.id': 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}'
        },
        postAttributeCollection: {
            '@odata.id': 'https://graph.microsoft.com/v1/identity/apiConnectors/{id}'
        }
    }
};

await client.api('/identity/b2xUserFlows')
    .post(b2xIdentityUserFlow);

```