---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c5891662b8cc5d6708fc316b4cd75b57c128fe4bccf789d754a4774fe89f024
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329473"
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
    .update(conversationThread);

```