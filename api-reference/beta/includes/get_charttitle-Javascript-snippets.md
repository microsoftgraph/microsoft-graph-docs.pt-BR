---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 73c57c7fee03b2cc1fa0e9f3836df25e2891ef7b
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472788"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/charts/{name}/title')
    .version('beta')
    .get();

```