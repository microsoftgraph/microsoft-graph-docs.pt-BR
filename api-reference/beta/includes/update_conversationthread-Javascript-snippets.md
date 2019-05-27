---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 15a8fab0d737bb34960c14ee6d2ebdd277221b8e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34475238"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  @odata.type:"#Microsoft.OutlookServices.ConversationThread",
  isLocked: true
};

let res = await client.api('/groups/{id}/threads/{id}')
    .version('beta')
    .update({conversationThread : conversationThread});

```