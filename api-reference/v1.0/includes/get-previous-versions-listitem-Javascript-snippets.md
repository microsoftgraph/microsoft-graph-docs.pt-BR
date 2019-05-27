---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 777726ed436ab5c4c8c11132d0fba0169dd73220
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462595"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions')
    .get();

```