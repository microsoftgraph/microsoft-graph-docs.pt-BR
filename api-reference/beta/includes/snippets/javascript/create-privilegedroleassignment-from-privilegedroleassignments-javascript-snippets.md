---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a68dd0c10d2886dfba47de87a1a191a1da6176fd
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720162"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  userId: "userId-value",
  roleId: "roleId-value"
};

let res = await client.api('/privilegedRoleAssignments')
    .version('beta')
    .post({privilegedRoleAssignment : privilegedRoleAssignment});

```