---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 544833d94db05c3bddec2a91c0b18e0c174cdf96
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChart = {
  id: 'id-value',
  height: 99,
  left: 99
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts')
    .version('beta')
    .post(workbookChart);

```