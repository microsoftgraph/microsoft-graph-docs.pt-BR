---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 059aaccfc6799f29ad663631a34d4213f9fce12f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707833"
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