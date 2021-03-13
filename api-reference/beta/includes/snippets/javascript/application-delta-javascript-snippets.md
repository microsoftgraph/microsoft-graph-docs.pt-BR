---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1575844fb471ec89c09bd895b5f080066222492
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let delta = await client.api('/applications/delta')
    .version('beta')
    .get();

```