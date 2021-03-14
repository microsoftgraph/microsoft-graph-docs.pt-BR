---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15e0267f029a3e4129fe45cceea9a9dc2284af74
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800464"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accept = {
  comment: 'comment-value',
  sendResponse: true
};

await client.api('/me/events/{id}/accept')
    .post(accept);

```