---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f5e20b56c25dd96962dc6ff8c43d8d79a760cfb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50790004"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const resultInfo = {
  value: [
    'externalId-value1',
    'externalId-value2'
  ]
};

await client.api('/security/tiIndicators/deleteTiIndicatorsByExternalId')
    .version('beta')
    .post(resultInfo);

```