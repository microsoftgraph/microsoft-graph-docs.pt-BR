---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19a4a24ffe0c408aadcd842034facedddf893884
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724769"
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
    .version('beta')
    .post({workbookTableColumn : workbookTableColumn});

```