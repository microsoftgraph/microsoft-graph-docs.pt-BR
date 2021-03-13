---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e44576d40b5b95fa31036a003ffc98e805b32411
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806982"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const approve = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/approve')
    .version('beta')
    .post(approve);

```