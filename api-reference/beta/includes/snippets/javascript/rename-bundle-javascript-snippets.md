---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79d559a16df7b5f606bc422d3138009f512eb5bf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  name: 'Shared legal agreements'
};

await client.api('/drive/items/{bundle-id}')
    .version('beta')
    .update(driveItem);

```