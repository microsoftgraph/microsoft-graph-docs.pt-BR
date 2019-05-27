---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84b82dcb6546990bfc8753f81d28d7335cdeadce
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles')
    .version('beta')
    .get();

```