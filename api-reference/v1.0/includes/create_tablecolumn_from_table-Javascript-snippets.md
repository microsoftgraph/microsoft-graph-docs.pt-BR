---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 913c9dc893370ae4f0bd2090289fa9a03e03944c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459839"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  id: 99,
  name: "name-value",
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns')
    .post({workbookTableColumn : workbookTableColumn});

```