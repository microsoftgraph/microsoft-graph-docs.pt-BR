---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: caadfe9c2a63e8cd8e4899b0571f152769d9abed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460963"
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
    .version('beta')
    .post(reply);

```