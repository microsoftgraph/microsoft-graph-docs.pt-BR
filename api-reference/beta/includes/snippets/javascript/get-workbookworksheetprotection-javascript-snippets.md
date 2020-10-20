---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 305c0ca0d0ea74cca054c228fa730c52f95dac87
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48618294"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/protection')
    .version('beta')
    .get();

```