---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 663e5575bf84db79e464a2269e7abfdcdebac3cf
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689835"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/chats/19:d65713bc498c4a428c71ef9353e6ce20@thread.v2/installedApps')
    .version('beta')
    .get();

```