---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7296b2c24031d81a4e21ceff60460c6bf81dae2a
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const teamsTab = {
  displayName: "My Contoso Tab - updated again"
};

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs/794f0e4e-4d10-4bb5-9079-3a465a629eff')
    .version('beta')
    .update(teamsTab);

```