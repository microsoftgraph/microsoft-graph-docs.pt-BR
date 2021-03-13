---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6c0233bc14a3c4bb2956564db496791d647bdbdf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause')
    .version('beta')
    .post();

```