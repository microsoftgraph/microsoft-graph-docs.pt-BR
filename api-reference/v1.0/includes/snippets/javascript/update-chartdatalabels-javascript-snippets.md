---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 047f400c76f70666b44355abf20356dee758d4f1
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492250"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartDataLabels = {
  position: "position-value",
  showValue: true,
  showSeriesName: true,
  showCategoryName: true,
  showLegendKey: true
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/dataLabels')
    .update({workbookChartDataLabels : workbookChartDataLabels});

```