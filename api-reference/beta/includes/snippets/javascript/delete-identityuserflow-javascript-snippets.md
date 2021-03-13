---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4dd9a419c3a5152431d9b9642349f02f5077285
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/userFlows/{id}')
    .version('beta')
    .delete();

```