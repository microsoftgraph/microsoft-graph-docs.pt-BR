---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb348d8c111a9b4c0dfbe2a95d64223984db2a96
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44334523"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appRoleAssignmentRequired: true
};

let res = await client.api('/servicePrincipals/{id}')
    .update(servicePrincipal);

```