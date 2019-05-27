---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a00f32a51b19da622ae9d25d664c9e882ae19dc7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34478535"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .post({workbookChartSeries : workbookChartSeries});

```