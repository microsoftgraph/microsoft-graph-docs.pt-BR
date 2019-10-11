---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5633e8c722e464dbdd8839a2947dccec99f8c83
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428741"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resultInfo = {
  value: [
    "id-value1",
    "id-value2"
  ]
};

let res = await client.api('/security/tiIndicators/deleteTiIndicators')
    .version('beta')
    .post(resultInfo);

```