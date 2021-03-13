---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: af8b1bbd075aba83a0cd41a4a0c444de5bac6f67
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801307"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ['read']
};

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .update(permission);

```