---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca173ab14d0771f499105eb3404adde588c151b4
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636201"
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
    .put(schedule);

```