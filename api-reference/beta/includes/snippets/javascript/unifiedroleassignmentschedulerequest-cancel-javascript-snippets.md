---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10068446f5903ac697c2a8fda1b8429ef40f13f8fcf38a178ae28ac45bfdbdf7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156401"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}/cancel')
    .version('beta')
    .post();

```