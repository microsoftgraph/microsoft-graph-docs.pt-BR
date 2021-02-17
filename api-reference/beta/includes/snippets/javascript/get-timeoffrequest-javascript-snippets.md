---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00702620add3b606386a66b9e24775eece7578a0
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274606"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .get();

```