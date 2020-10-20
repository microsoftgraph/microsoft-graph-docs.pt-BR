---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d537c365d2e65bd6d1301f6656d85775429eda0
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609282"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{servicePrincipalId}/synchronization/jobs/{jobId}/schema')
    .version('beta')
    .header('Authorization','Bearer {Token}')
    .get();

```