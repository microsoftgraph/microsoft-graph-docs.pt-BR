---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 94079133aa4036c72fb2914d0c1a7f676c8880aa
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790979"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let conversation = await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .get();

```