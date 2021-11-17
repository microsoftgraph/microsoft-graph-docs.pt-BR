---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d4702f713a29a038f1ce5fe4cfd16f6b38d569a2828ddfa6fe1f2d057fd9ef9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementActionTenantDeploymentStatuses = await client.api('/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses')
    .version('beta')
    .get();

```