---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b79ca1aea181646f60c6a72126738bdeb8a692ed
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797432"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const decline = {
  message: 'message-value'
};

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}/decline')
    .version('beta')
    .post(decline);

```