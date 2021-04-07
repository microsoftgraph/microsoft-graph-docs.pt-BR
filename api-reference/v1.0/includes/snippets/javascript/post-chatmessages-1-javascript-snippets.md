---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a9664b362fcf2b4677088991e081f88d0f1866ed
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612000"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
     content: 'Hello world'
  }
};

await client.api('/chats/19:2da4c29f6d7041eca70b638b43d45437@thread.v2/messages')
    .post(chatMessage);

```