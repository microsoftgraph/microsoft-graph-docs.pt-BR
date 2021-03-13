---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fd9e0d69395f8c7e266e47a3c238bbf15661213
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let identitySecurityDefaultsEnforcementPolicy = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .version('beta')
    .get();

```