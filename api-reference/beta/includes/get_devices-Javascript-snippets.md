---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f01abeaeb4f046c033526ad8737b291a4ee1c2df
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/devices')
    .version('beta')
    .get();

```