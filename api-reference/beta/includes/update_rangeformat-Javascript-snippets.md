---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7d2543ae716094b9a6cfefbda1c3c3afb92e071d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461738"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  verticalAlignment: "Top",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$A$1')/format')
    .version('beta')
    .update({workbookRangeFormat : workbookRangeFormat});

```