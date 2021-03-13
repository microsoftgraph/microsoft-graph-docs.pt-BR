---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85755ed4544218c4e58f8dfa86d1426e225194f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791711"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oauth2PermissionGrants = await client.api('/oauth2PermissionGrants')
    .version('beta')
    .get();

```