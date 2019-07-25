---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 05d544252360cf943b34558e37e0b5e5cf363bf4
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookWorksheet = {
  name: "name-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/add')
    .version('beta')
    .post(workbookWorksheet);

```