---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcfc6b6f0d660256d3764849facd6330d1e498ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/messages/{id}/unsubscribe')
    .version('beta')
    .post();

```