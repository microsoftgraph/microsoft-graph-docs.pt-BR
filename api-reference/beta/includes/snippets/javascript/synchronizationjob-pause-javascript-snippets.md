---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 49b19dd1144a62850c34828722c151376493617e
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476195"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/pause')
    .version('beta')
    .post();

```