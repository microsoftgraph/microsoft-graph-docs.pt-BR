---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08db622dc0570fbbf337b8e51636bb447812c68c58669e299533d5186e89b2b5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273312"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementActionTenantDeploymentStatus = await client.api('/tenantRelationships/managedTenants/managementActionTenantDeploymentStatuses/{managementActionTenantDeploymentStatusId}')
    .version('beta')
    .get();

```