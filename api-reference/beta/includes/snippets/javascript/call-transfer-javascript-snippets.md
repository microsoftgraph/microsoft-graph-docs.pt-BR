---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a03227d1c8b2bb6eced20c7808362cb124fa9c6
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756065"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const transfer = {
  transferTarget: {
    endpointType: "default",
    identity: {
        phone: {
          @odata.type: "#microsoft.graph.identity",
          id: "+12345678901"
        }
    },
    languageId: "languageId-value",
    region: "region-value"
  },
  clientContext: "9e90d1c1-f61e-43e7-9f75-d420159aae08"
};

let res = await client.api('/communications/calls/{id}/transfer')
    .version('beta')
    .post(transfer);

```