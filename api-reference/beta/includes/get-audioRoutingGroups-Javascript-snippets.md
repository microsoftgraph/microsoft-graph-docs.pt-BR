---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b8edb3a31ae5e0132b784e96bfd169856d8bda7b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/app/calls/{id}/audioRoutingGroups')
    .version('beta')
    .get();

```