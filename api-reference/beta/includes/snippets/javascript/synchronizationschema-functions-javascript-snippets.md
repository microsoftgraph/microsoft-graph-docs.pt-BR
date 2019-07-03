---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30941e358ffa975bcabbd6ac189f216d91215b5c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476241"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/functions')
    .version('beta')
    .get();

```