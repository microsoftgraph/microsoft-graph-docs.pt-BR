---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9802016782c35e635b31e0409cb0f79a26899ea2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445921"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/subscribedSkus/{id}')
    .version('beta')
    .get();

```