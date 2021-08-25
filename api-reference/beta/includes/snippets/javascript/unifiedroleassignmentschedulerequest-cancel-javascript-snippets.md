---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 016d02c70fe928cbff54d72f2fd6a8cceef1ee7f
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516003"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/15fec3d4-64b1-4b03-beb7-f1ba6dddf6cc/cancel')
    .version('beta')
    .post();

```