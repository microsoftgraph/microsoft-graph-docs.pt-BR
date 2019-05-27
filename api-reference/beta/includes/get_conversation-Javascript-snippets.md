---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60cd1d4c1d13ebb7dda369ad8fa7506a531dae98
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472473"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/conversations/{id}')
    .version('beta')
    .get();

```