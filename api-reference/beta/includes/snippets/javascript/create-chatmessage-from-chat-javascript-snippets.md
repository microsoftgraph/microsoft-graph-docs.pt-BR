---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 197dd8047b87d1b2030b88dedb3dd7342187c616
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     content: "Hello world"
  }
};

let res = await client.api('/chats/{id}/messages')
    .version('beta')
    .post(chatMessage);

```