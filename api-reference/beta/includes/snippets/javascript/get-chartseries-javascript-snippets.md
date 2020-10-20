---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31320aa1a4d6e715af27921f1d3016dfee9810c1
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48610495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series/{undefined}')
    .version('beta')
    .get();

```