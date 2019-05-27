---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a113ed8c7b0d5a1e519b1b44e1b573d39c9741f5
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34443107"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: "reason-value",
  ticketNumber: "ticketNumber-value",
  ticketSystem: "ticketSystem-value"
};

let res = await client.api('/privilegedRoleAssignments/{id}/makePermanent')
    .version('beta')
    .post(privilegedRoleAssignment);

```