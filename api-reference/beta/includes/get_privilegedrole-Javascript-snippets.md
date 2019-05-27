---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be16d9d73cbf393913fbf46533bd566aed336c44
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/privilegedRoles/{id}')
    .version('beta')
    .get();

```