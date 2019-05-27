---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18900b9e82a6de93d344427b9a6fec55e13bf4f3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFormat = {
  columnWidth: 135,
  horizontalAlignment: "Right",
  verticalAlignment: "Top",
  rowHeight: 49,
  wrapText: false
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format')
    .version('beta')
    .update({workbookRangeFormat : workbookRangeFormat});

```