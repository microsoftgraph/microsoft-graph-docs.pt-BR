---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3bfbd7bca48012daa28c08003b3b27d286bb11bc5847425032ffefef90cb60a9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216556"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleEligibilityScheduleRequests = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests')
    .version('beta')
    .get();

```