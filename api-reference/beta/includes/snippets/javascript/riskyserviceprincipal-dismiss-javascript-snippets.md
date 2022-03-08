---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bfb70792481dbf246c41a28ed3d69cf83eb0b0b
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336995"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const dismiss = {
  servicePrincipalIds: [
    '9089a539-a539-9089-39a5-899039a58990'
  ]
};

await client.api('/identityProtection/riskyServicePrincipals/dismiss')
    .version('beta')
    .post(dismiss);

```