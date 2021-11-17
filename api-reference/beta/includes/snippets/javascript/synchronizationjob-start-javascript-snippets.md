---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a63e2f794c4934c4fb4bdd7225d0342152a022fd9483b098d6f4539a98798008
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216280"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/start')
    .version('beta')
    .post();

```