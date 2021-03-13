---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad5daf0a44438e8265a8dd61abdce42eb5b33a53
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800662"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoles/{id}/selfDeactivate')
    .version('beta')
    .post();

```