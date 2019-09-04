---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11a782ed75a3f5fcfb7e394af534f939ef6a7beb
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636328"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const workbookTableColumn = {
  index: 3
};

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/columns/itemAt')
    .post(workbookTableColumn);

```