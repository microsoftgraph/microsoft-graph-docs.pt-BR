---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9747afeef481c886d39ab467c35d45fe0f79f98
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40863614"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffRequest = {
  message: "message-value"
};

let res = await client.api('/teams/{id}/schedule/timeOffRequests/decline')
    .version('beta')
    .post(timeOffRequest);

```