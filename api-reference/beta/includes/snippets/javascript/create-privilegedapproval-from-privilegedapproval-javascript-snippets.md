---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dc585a4f809ad17b126d561beaed2ac487d3a3874b4dc2458aebf44e96478aa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101584"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedApproval = {
  userId: 'userId-value',
  roleId: 'roleId-value',
  approvalType: 'approvalType-value',
  approvalState: 'approvalState-value',
  approvalDuration: 'datetime-value'
};

await client.api('/privilegedApproval')
    .version('beta')
    .post(privilegedApproval);

```