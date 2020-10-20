---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98496ab340dbe13041342fb85d0caed038899a96
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48621748"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/seriesaxis/format/line/clear')
    .version('beta')
    .post();

```