---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d81f7fc46ab97e1c23aa493da4028958a755dc04
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945153"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appRoleAssignment = {
  principalId: "principalId-value",
  resourceId: "resourceId-value",
  appRoleId: "appRoleId-value"
};

let res = await client.api('/groups/{id}/appRoleAssignments')
    .version('beta')
    .post(appRoleAssignment);

```