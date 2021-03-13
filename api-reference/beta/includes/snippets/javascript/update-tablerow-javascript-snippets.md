---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1e7ed168aa1be76bd2ee02b1c542fdc7b8db0084
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableRow = {
  index: 99,
  values: 'values-value'
};

await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}')
    .version('beta')
    .update(workbookTableRow);

```