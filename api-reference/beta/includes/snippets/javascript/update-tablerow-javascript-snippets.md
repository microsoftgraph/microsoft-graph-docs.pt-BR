---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e41f66722bfa31f83f5b40fc95ea0a5fe69e92d4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35724593"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 99,
  values: "values-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .version('beta')
    .update({workbookTableRow : workbookTableRow});

```