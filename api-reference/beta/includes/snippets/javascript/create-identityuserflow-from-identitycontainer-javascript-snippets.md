---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6643fd6e31ac6d0c67b752c5009bd2e0e32f64b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274822"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityUserFlow = {
  id: "Pol1",
  userFlowType: "signUpOrSignIn",
  userFlowTypeVersion: 1
};

let res = await client.api('/identity/userFlows')
    .version('beta')
    .post(identityUserFlow);

```