---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 336f1277513edca4086dd76346b47e16382b65b5
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49843666"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const channel = {
    displayName: "UpdateChannelModeration",
    description: "Update channel moderation.",
    moderationSettings: {
        userNewMessageRestriction: "moderators",
        replyRestriction: "everyone",
        allowNewMessageFromBots: true,
        allowNewMessageFromConnectors: true
    }
};

let res = await client.api('/teams/{team-id}/channels/{channel-id}')
    .version('beta')
    .update(channel);

```