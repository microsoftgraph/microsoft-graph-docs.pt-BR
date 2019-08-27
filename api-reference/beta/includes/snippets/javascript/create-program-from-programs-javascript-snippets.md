---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6230f92b1ee69ba857a5faacbfdeac01005f3614
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636226"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const program = {
    displayName: "testprogram3",
    description: "test description"
};

let res = await client.api('/programs')
    .version('beta')
    .post(program);

```