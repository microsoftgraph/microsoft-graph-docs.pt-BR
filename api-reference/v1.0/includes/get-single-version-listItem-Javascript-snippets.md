---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba3b36dfe9edf6be530b5e523e4bb24379350f0e
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34455672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/sites/{site-id}/lists/{list-id}/items/{item-id}/versions/{version-id}')
    .get();

```