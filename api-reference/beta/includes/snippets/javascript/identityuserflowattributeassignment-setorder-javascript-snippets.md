---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5734c4f14048934834cfb390aeee1d732c20b416
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const setOrder = {
  newAssignmentOrder: {
    order: [
        "City",
        "extension_GUID_ShoeSize"
    ]
  }
};

let res = await client.api('/identity/b2cUserFlows/{id}/userAttributeAssignments/setOrder')
    .version('beta')
    .post(setOrder);

```