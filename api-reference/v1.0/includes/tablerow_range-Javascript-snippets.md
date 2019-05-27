---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86b284558aa67d9b9186175be4a99f94bdde4149
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34449930"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/tables/{id|name}/rows/{index}/range')
    .get();

```