---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c6b11560f250a5ba16581d8172da7614ad008ee1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803403"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover')
    .version('beta')
    .post();

```