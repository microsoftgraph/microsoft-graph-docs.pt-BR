---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7c97a5fe309fbab9a5cc6b57d3900b025a23bda0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775490"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .version('beta')
    .delete();

```