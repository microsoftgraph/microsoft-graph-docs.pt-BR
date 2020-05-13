---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc3e30237b94a8fa4e2747f261e045653e7950a5
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "44219201"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .delete();

```