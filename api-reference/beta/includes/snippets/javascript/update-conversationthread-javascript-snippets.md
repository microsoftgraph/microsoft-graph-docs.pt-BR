---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 297a2cc990f9b02df42f170783cb77974bddf278
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800173"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  '@odata.type':'#Microsoft.OutlookServices.ConversationThread',
  isLocked: true
};

await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .update(conversationThread);

```