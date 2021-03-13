---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2eaae307d1b979b62b8406b4d41df776376c5458
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796664"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delegatedPermissionClassifications = await client.api('/servicePrincipals/{id}/delegatedPermissionClassifications')
    .version('beta')
    .get();

```