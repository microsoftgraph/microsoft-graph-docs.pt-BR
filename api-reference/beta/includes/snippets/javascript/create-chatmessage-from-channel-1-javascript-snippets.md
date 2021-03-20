---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43a34d286865d9d402547bec1cf09a5b6fbbf8d6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948263"
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
    .version('beta')
    .post(chatMessage);

```