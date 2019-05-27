---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 593f3ed6b6b821dc48fd8bd60dbbab0f208fe9d0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452483"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directory/deletedItems/microsoft.graph.group')
    .get();

```