---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8443f1d294d01cb7fa7f9e742007534858d23f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447828"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .version('beta')
    .get();

```