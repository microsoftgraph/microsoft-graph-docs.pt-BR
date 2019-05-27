---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca884fea066ef5075fedfbb579c9e07be86bb557
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34471477"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/endpoints')
    .version('beta')
    .get();

```