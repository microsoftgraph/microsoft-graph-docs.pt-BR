---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9abf4965c1442928ccd9ae66b7869681b00cc2a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607700"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/title')
    .version('beta')
    .get();

```