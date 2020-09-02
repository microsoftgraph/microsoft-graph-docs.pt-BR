---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4821034685033141076cb4a1a3b7ad2d5dabbb81
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330391"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const set = {
  description: "mySet"
};

let res = await client.api('/termStore/sets/{setId}')
    .version('beta')
    .update(set);

```