---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f1385215182e4448631febab2dfddc5fd965543
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802223"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/invalidateAllRefreshTokens')
    .version('beta')
    .post();

```