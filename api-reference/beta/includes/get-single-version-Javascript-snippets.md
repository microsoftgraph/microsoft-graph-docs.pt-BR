---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55ae26fb4f3dcf1d16bb55d8a8ca84fadb5f23f6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474580"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/drive/items/{item-id}/versions/{version-id}')
    .version('beta')
    .get();

```