---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 20f68fd6f3d2c5d6953fb7b16a223cd614e647ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787344"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identity/conditionalAccess/policies/{id}')
    .version('beta')
    .delete();

```