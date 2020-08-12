---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 24c6c955b34fab32ac3e9c118bd858d15eb347ea
ms.sourcegitcommit: 8e18d7fe3c869b2fd48872365116175d3bdce1b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/12/2020
ms.locfileid: "46643781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{jobId}/start')
    .version('beta')
    .post();

```