---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 16997fc4707ef4fb7e1920410d94ab8c1abde290
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957889"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequest = await client.api('/teams/{teamId}/schedule/offerShiftRequests/{offerShiftRequestId}')
    .version('beta')
    .get();

```