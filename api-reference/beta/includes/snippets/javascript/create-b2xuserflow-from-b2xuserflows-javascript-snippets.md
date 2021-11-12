---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f766c300f5a72b601a82c87d3c1924edf6f344df0d9472e585bb78bd14e001eb
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274750"
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
    .version('beta')
    .post(b2xIdentityUserFlow);

```