---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 939a67f41f4cde4c09cef3fe8cd2cf76f537090b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799064"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline')
    .version('beta')
    .post(decline);

```