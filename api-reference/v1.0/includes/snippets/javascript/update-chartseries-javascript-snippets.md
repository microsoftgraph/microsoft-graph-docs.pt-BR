---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd2c84facc421389f981b6c748614fa35d6565f82830188705c934a11f809769
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330077"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartSeries = {
  name: 'name-value'
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}')
    .update(workbookChartSeries);

```