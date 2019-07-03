---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98496ab340dbe13041342fb85d0caed038899a96
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463434"
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