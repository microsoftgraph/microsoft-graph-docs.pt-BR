---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 605de3c4c12069502107761a0a6d25904db31dee
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843651"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookRangeFill = {
  color: "#0000FF"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/Sheet1/range(address='$C$1')/format/fill')
    .update({workbookRangeFill : workbookRangeFill});

```