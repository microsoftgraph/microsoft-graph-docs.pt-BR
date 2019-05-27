---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f8cb1f2e23b095557abd15ad53fd4d6e1506aa78
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{id}/workbook/application')
    .version('beta')
    .get();

```