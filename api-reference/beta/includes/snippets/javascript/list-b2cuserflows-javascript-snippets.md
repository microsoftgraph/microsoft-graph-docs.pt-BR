---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8554bae4a6301d1ab31c240579d8be580d075446
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329808"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows')
    .version('beta')
    .get();

```