---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9734eacf423dd3a945cf8ade5e7d129c43b0ca35de8625fd48e99a5e305e02f6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57157520"
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
    .post(decline);

```