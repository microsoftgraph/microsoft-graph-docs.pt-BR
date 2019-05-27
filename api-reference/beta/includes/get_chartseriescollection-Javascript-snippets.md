---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcc7255557ffd8d1ca7183c4c5f55be0a9b54363
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472879"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/series')
    .version('beta')
    .get();

```