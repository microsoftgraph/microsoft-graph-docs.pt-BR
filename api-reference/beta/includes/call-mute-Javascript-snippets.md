---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f12a47f2883fdd42ef1d2e257f65328ae548d553
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/mute')
    .version('beta')
    .post(CommsOperation);

```