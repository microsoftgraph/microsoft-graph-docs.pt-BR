---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 58dca924f18690aaeefe8e8fca10637e9c10345e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781980"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityApiConnector = {
    '@odata.id': 'https://graph.microsoft.com/beta/identity/apiConnectors/{id}'   
};

await client.api('/identity/b2xUserFlows/B2X_1_testuserflow/apiConnectorConfiguration/postFederationSignup/$ref')
    .version('beta')
    .put(identityApiConnector);

```