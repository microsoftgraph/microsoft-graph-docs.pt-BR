---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b4deb661254394b21cb79017b5f287901954feb1a883fd8bdee4282d33265d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271897"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  reason: 'reason-value',
  ticketNumber: 'ticketNumber-value',
  ticketSystem: 'ticketSystem-value'
};

await client.api('/privilegedRoleAssignments/{id}/makePermanent')
    .version('beta')
    .post(privilegedRoleAssignment);

```