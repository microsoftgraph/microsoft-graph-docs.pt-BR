---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 237e520f72c1ba5722dd1206144d8afa28587f7a
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807787"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2cIdentityUserFlow = {
    id: 'Customer',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 3
};

await client.api('/identity/b2cUserFlows')
    .version('beta')
    .post(b2cIdentityUserFlow);

```