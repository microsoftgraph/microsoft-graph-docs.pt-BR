---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecb524f6a91fb64d5c728924a102c4a27b09b68e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35499223"
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