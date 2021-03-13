---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 93d5ad13881980113013a570bff2d2e7ab7e4be7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50793046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  topic: 'topic-value',
  posts: [{
      body: {
        contentType: 'html',
        content: 'this is body content'
      }
  }]
};

await client.api('/groups/{id}/conversations/{id}/threads')
    .version('beta')
    .post(conversationThread);

```