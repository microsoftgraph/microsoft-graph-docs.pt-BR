---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89be91ecd13a3a77e2efedf77f1675f05f6dddc2
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let workbookChartSeries = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .get();

```