---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6fc6c8ea1e9c5b3c27d8895373569570ffc2837
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964260"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    content: 'Hello World'
  }
};

await client.api('/teams/{id}/channels/{id}/messages')
    .post(chatMessage);

```