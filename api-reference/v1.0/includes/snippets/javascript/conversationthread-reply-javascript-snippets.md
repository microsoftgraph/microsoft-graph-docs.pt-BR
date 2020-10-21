---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c63bfcfd7a7c128991b2c19c24d1a7a69ba9330
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: "",
      content: "content-value"
    }
  }
};

let res = await client.api('/groups/{id}/threads/{id}/reply')
    .post(reply);

```