---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a6bfc810fade102c78bf95c967f775dcd6ef06b
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946011"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let offerShiftRequests = await client.api('/teams/{teamId}/schedule/offerShiftRequests')
    .version('beta')
    .get();

```