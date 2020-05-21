---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1fd0d9fe99c2e3c93f771cbb3a587521dad3ee1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44336227"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/appRoleAssignedTo')
    .get();

```