---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9fa70ea4a9354915d54777ef8ec3fb7c3ef08b70
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timeOffRequests/{timeOffRequestId}')
    .version('beta')
    .delete();

```