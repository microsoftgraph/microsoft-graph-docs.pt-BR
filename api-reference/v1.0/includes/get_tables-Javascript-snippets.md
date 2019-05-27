---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff3943137225eeb44c9ffe9c67fe744c584d2917
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34465710"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/worksheets/{id|name}/tables')
    .get();

```