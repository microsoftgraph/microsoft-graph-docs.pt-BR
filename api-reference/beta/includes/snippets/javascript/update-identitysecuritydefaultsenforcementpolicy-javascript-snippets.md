---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40b73064036dc4c9fbf059e4ffce757d55c4a8c7
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946998"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identitySecurityDefaultsEnforcementPolicy = {
  isEnabled: false
};

let res = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .version('beta')
    .update(identitySecurityDefaultsEnforcementPolicy);

```