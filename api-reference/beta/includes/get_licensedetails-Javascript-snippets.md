---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47abdb1a1d426829eb65dbe213f2280ba820e6e9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449213"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/licenseDetails')
    .version('beta')
    .get();

```