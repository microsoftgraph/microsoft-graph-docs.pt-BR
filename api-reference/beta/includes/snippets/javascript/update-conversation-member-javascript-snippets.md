---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8a5090b8939aa1429b31ec5d7b7a7741f2428a878054284d01f37a5df11142a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271861"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
  '@odata.type':'#microsoft.graph.aadUserConversationMember',
  roles: ['owner']
};

await client.api('/teams/{id}/channels/{id}/members/{id}')
    .version('beta')
    .update(conversationMember);

```