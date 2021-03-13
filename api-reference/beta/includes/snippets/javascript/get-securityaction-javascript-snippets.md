---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc4d015003eec6fa5d05ffe06c74db990ccfab43
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50794382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let securityAction = await client.api('/security/securityActions/{id}')
    .version('beta')
    .get();

```