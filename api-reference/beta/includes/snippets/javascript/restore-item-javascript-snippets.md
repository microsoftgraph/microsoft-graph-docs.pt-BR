---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 110c1ecdf3ea9f42c5b0fcb565074e92d1807bc0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801796"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const driveItem = {
  parentReference: {
    id: 'String',
  },
  name: 'String'
};

await client.api('/me/drive/items/{item-id}/restore')
    .version('beta')
    .post(driveItem);

```