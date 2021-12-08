---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6d2d630909dcbf9686df5e178f33e6e41313df8f
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61346714"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName: 'Connected organization new name',
  description: 'Connected organization new description',
  state: 'configured'
};

await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/{id}')
    .update(connectedOrganization);

```