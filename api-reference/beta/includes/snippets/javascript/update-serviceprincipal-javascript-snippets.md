---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51168cc9a72bcf087fc9b744be27d3ded8509b075d223e7d63911caca9705ea0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const servicePrincipal = {
  appRoleAssignmentRequired: true
};

await client.api('/servicePrincipals/{id}')
    .version('beta')
    .update(servicePrincipal);

```