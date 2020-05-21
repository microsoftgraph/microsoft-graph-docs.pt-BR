---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: defa460339215f1e65fbbf603ac3048c08e58d53
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333798"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```