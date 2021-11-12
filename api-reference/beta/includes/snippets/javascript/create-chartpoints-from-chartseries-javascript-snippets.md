---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82fa6630ea7a694f2aec9b58e508f070e9f816e8e195690659a8ac1178a27a13
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156265"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}/points')
    .version('beta')
    .post(workbookChartPoint);

```