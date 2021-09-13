---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85024a2864835570473034d45276dad3a58ce8adf43e2d95cb91c0b63d0b0580
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57407719"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartAxisTitle = {
  text: 'text-value',
  visible: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/title')
    .update(workbookChartAxisTitle);

```