---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7fc6eab9576787060d8cdac141dec47b54be37c7a47964dc5cd01738b2c25762
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{servicePrincipal-id}/appRoleAssignments/{appRoleAssignment-id}')
    .version('beta')
    .delete();

```