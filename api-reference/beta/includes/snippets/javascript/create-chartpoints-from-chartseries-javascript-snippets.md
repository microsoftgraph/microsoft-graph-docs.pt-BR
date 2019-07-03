---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37d9ad3cff386811b3fcce4ddabca7aea0a427e6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518895"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points')
    .version('beta')
    .post({workbookChartPoint : workbookChartPoint});

```