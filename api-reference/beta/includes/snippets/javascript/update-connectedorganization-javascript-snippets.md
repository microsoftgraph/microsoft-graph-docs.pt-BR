---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cafc2e4d5464e3aa4c2a8a3c0ed63f976240afc4
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47331101"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName:"Connected organization new name",
  description:"Connected organization new description",
  state:"configured"
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .version('beta')
    .update(connectedOrganization);

```