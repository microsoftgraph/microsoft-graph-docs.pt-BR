---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c51d0ee64acd51974f5d02b76d734cd3f9a83307
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58516018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentSchedule = await client.api('/roleManagement/directory/roleAssignmentSchedules/226faf5f-61b4-40bb-8726-52e48ec914de')
    .version('beta')
    .get();

```