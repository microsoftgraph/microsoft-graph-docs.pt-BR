---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f41aa39858fe724ee5be0d23af8ef23ea3592f8592344239309d3c59e2843335
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const b2xIdentityUserFlow = {
    id: 'Partner',
    userFlowType: 'signUpOrSignIn',
    userFlowTypeVersion: 1
};

await client.api('/identity/b2xUserFlows')
    .post(b2xIdentityUserFlow);

```