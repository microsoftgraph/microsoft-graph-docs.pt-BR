---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 173f67e109d9e8cf81ebdf06f3d22aaf2bff5efc
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  Comment: "Cancelling for this week due to all hands"
};

let res = await client.api('/me/events/{id}/cancel')
    .version('beta')
    .post(cancel);

```