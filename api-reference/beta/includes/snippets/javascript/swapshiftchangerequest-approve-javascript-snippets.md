---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7cd85fa72aadae18343d5c678650b3fbc62fc613
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796515"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/approve')
    .version('beta')
    .post(approve);

```