---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecb524f6a91fb64d5c728924a102c4a27b09b68e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35714029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tentativelyAccept = {
  comment: "comment-value",
  sendResponse: true
};

let res = await client.api('/me/events/{id}/tentativelyAccept')
    .version('beta')
    .post(tentativelyAccept);

```