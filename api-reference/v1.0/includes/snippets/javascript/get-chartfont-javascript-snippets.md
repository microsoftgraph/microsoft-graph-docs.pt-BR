---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d239acf2b05002382994e9b69b204e9f9bbacd7b
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48607976"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueAxis/format/font')
    .get();

```