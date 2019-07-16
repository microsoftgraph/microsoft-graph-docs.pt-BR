---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f18f528747d77c9a4485aae87560d2d3c69efe7a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35736591"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxis = {
  majorUnit: {
  },
  maximum: {
  },
  minimum: {
  }
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis')
    .update({workbookChartAxis : workbookChartAxis});

```