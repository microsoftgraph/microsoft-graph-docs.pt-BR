---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9405f1a94d8d497de7b8210b1255d5603adca1f8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806217"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/education/classes/11021/assignments/19002/submissions/850f51b7/unsubmit')
    .version('beta')
    .post();

```