---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aaf21476c036a8ec6c133ce277a62f276b1cddec
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522908"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationMember = {
    @odata.type: "#microsoft.graph.aadUserConversationMember",
    roles: ["owner"],
    user@odata.bind: "https://graph.microsoft.com/v1.0/users('8b081ef6-4792-4def-b2c9-c363a1bf41d5')"
};

let res = await client.api('/teams/ee0f5ae2-8bc6-4ae5-8466-7daeebbfa062/members')
    .post(conversationMember);

```