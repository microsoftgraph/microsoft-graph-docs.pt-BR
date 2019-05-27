---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86efc52ecf3f329f631cbefb8a9ebe8875796a12
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448522"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}')
    .version('beta')
    .get();

```