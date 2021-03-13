---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 771decfc46ecb4c2a367daee0e7fbc89e0f9bcb0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796981"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/education/classes/delta')
    .version('beta')
    .get();

```