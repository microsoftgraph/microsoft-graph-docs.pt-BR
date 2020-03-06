---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78f5990b7ee3e83f5266ba0a845f4f543dc82e5c
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636326"
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
    .post(workbookTableRow);

```