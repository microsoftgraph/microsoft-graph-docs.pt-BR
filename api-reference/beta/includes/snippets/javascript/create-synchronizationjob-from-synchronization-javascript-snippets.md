---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb53ac1146d30736081d51ac7acb9e1ebf2ded0198f184fafbfa378752f5451f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102580"
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