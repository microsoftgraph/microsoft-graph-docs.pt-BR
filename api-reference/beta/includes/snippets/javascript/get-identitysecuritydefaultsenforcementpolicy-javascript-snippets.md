---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 856f1bf80509ec352687c88fadc1e19c19256f67
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947054"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/identitySecurityDefaultsEnforcementPolicy')
    .version('beta')
    .get();

```