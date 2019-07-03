---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 059aaccfc6799f29ad663631a34d4213f9fce12f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463430"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  index: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/ItemAt')
    .version('beta')
    .post({workbookChartSeries : workbookChartSeries});

```