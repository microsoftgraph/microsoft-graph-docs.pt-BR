---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcdec3e0aa1b5e2363e320b5efda6fab22a89af3
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689927"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/tabs')
    .version('beta')
    .expand('teamsApp')
    .get();

```