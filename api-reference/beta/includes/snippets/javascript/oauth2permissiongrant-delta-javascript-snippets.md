---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5772c2572fb91d2c4a5ed4aef480371b00d1e77e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795323"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/oauth2PermissionGrants/delta')
    .version('beta')
    .get();

```