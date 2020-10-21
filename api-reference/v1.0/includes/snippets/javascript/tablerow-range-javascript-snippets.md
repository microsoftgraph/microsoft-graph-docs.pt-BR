---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86b284558aa67d9b9186175be4a99f94bdde4149
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614069"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range')
    .get();

```