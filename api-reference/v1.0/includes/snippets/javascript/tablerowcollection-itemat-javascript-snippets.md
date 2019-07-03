---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3d8b8cb2a36889c0bcb323f1f13f93461b0496aa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492268"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 4
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/itemAt')
    .post({workbookTableRow : workbookTableRow});

```