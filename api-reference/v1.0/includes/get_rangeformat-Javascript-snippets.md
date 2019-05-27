---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d6869dad0cf2d67166a548241d464558f7f1fe89
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434987"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/names/{name}/range/format')
    .get();

```