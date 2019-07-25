---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 380160445735d725747814b74cf68668ebc5e43e
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716954"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const schedule = {
  enabled: true,
  timeZone: "America/Chicago"
};

let res = await client.api('/teams/{teamId}/schedule')
    .version('beta')
    .put({schedule : schedule});

```