---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cafcc2554ad6603eb1565d0b011c228208748d37d6021f3885ea25015df0359a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102931"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const chatMessage = {
  body: {
    contentType: 'html',
    content: 'Hello World <at id=\"0\">Jane Smith</at>'
  },
  mentions: [
    {
      id: 0,
      mentionText: 'Jane Smith',
      mentioned: {
        user: {
          displayName: 'Jane Smith',
          id: 'ef1c916a-3135-4417-ba27-8eb7bd084193',
          userIdentityType: 'aadUser'
        }
      }
    }
  ]
};

await client.api('/teams/fbe2bf47-16c8-47cf-b4a5-4b9b187c508b/channels/19:4a95f7d8db4c4e7fae857bcebe0623e6@thread.tacv2/messages')
    .version('beta')
    .post(chatMessage);

```