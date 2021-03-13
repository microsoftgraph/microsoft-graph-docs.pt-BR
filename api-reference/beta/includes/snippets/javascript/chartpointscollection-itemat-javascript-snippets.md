---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82f2b2a5172c19d0cb51107cb12b8239a1e197ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796856"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt')
    .version('beta')
    .post(workbookChartPoint);

```