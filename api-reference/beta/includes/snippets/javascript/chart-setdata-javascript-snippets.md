---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8adc5982def3af9cffd813ce9ec9067b2ead119b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35708367"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setData = {
  sourceData: "sourceData-value",
  seriesBy: "seriesBy-value"
};

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/setData')
    .version('beta')
    .post(setData);

```