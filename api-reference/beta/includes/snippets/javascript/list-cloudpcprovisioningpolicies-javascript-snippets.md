---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 546b548fc8ca0ed3738d2dd1e8d0ea7cff42a0db
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522564"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/deviceManagement/virtualEndpoint/provisioningPolicies')
    .version('beta')
    .get();

```