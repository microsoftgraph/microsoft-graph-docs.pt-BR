---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc3c38d89208857d5c5885bed7332f0ffb97125f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34473061"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/datalabels')
    .version('beta')
    .get();

```