---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 431883ce34a116b4edb7829038e644cc917ee56d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786300"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: {
  }
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/ItemAt')
    .version('beta')
    .post(workbookTableColumn);

```