---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fafd8f5dbedf48b1aa1209234a818952e7631fbb
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35735254"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points')
    .post({workbookChartPoint : workbookChartPoint});

```