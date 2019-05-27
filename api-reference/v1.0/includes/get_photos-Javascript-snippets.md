---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee2ff962a98f4a4d0cdf3b2429d9131a8da22787
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451120"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/photos')
    .get();

```