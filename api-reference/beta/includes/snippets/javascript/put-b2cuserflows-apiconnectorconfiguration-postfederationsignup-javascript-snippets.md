---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c93f5ecd1478467d1a526df92fed0bafb12c2eba
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794084"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    '@odata.id': 'https://graph.microsoft.com/beta/identity/apiConnectors/{id}'   
};

await client.api('/identity/b2cUserFlows/B2C_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref')
    .version('beta')
    .put(identityApiConnector);

```