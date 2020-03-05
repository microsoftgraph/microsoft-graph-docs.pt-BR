---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3fd6cf96b14ab8c2e5418be86062a58b9803ca76
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280642"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "message-value"
};

let res = await client.api('/teams/{id}/schedule/swapShiftsChangeRequests/{swapShiftChangeRequestId}/decline')
    .version('beta')
    .post(decline);

```