---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 061ce73a3997a8a969706d39ab3e89795755c933
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953884"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffRequests = await client.api('/teams/{teamId}/schedule/timeOffRequests')
    .version('beta')
    .get();

```