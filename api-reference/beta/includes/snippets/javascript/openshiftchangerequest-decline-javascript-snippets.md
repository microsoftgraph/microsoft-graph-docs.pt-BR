---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 549562e96996e827f51001f45ff364dd1052463f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50447855"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: "message-value"
};

let res = await client.api('/teams/{id}/schedule/openShiftChangeRequests/{openShiftChangeRequestId}/decline')
    .version('beta')
    .post(decline);

```