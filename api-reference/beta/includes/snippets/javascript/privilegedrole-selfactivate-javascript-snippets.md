---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3eeeb9fcc67408d97cff54e2a6ff7baa965ecf1b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787459"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: 'reason-value',
  duration: 'duration-value',
  ticketNumber: 'ticketNumber-value',
  ticketSystem: 'ticketSystem-value'
};

await client.api('/privilegedRoles/{id}/selfActivate')
    .version('beta')
    .post(privilegedRoleAssignment);

```