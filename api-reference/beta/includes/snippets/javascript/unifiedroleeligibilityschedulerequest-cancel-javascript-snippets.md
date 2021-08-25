---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 34d981d423f7620bdec83a6f4aa450415e8ebefe
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516029"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/532bef1f-c677-4564-aa6f-811444a4f018/cancel')
    .version('beta')
    .post();

```