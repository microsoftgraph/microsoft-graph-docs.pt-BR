---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fafd8f5dbedf48b1aa1209234a818952e7631fbb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492372"
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