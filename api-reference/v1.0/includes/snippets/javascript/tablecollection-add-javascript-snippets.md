---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1765d3e206d0f2c2442da0959eb31fb3325b366
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35731510"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTable = {
  address: "Sheet1!A1:D5",
  hasHeaders: true
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/add')
    .post(workbookTable);

```