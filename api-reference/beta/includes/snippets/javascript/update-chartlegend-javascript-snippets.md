---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55f276c540db36b024de587c97397ff8da8ea6082432b893239f1ffcc6e9fa0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookChartLegend = {
  visible: true,
  position: 'position-value',
  overlay: true
};

await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/legend')
    .version('beta')
    .update(workbookChartLegend);

```