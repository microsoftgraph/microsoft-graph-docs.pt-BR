---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c197809fa5ef2a7e0a5b40bcfddc91ff9c8a3838
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47329772"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identity/b2cUserFlows/{id}')
    .version('beta')
    .delete();

```