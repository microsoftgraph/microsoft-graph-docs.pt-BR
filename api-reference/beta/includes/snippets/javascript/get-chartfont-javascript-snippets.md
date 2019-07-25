---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4452531282d67f739cacbfa18992109bb25b745
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708197"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/axes/valueaxis/format/font')
    .version('beta')
    .get();

```