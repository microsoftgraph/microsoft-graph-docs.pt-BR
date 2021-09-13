---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e652a78fa2c85a93ddcde0bbe34c9437bd55f36f5759a951e9f5a2db88483590
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartPoint = {
  index: 8
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{series-id}/points/itemAt')
    .post(workbookChartPoint);

```