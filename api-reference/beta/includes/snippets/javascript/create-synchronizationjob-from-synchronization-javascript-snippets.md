---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dcab369d83561167e0ea7325489e03b0785a735f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775092"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const synchronizationJob = {
    templateId: 'BoxOutDelta'
};

await client.api('/servicePrincipals/{id}/synchronization/jobs')
    .version('beta')
    .post(synchronizationJob);

```