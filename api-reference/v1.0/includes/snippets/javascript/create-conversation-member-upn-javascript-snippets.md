---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0059f96bdd7bf1d978e895435aeee6d8a2441f5c
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60696536"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    '@odata.type': '#microsoft.graph.aadUserConversationMember',
    'user@odata.bind': 'https://graph.microsoft.com/v1.0/users/jacob@contoso.com',
    visibleHistoryStartDateTime: '2019-04-18T23:51:43.255Z',
    roles: ['owner']
};

await client.api('/chats/19:cf66807577b149cca1b7af0c32eec122@thread.v2/members')
    .post(conversationMember);

```