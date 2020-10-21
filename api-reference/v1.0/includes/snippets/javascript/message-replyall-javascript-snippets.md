---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4fe3bde5536979c95d3d6f6a03761ed1d92df87a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48608426"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const replyAll = {
  comment: "comment-value"
};

let res = await client.api('/me/messages/{id}/replyAll')
    .post(replyAll);

```