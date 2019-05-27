---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cf58381c73fa208441827a6098e78ae3c2377fe5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451886"
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

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points/ItemAt')
    .version('beta')
    .post({workbookChartPoint : workbookChartPoint});

```