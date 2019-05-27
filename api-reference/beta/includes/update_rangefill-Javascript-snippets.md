---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f35aa75d9c36b0d8d119ec0d4a3cd289e91e0967
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34461864"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "color-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format/fill')
    .version('beta')
    .update({workbookRangeFill : workbookRangeFill});

```