---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6ed1bc357af71482b10975beddc4417ef4fd28b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel')
    .version('beta')
    .post();

```