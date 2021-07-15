---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 467fe0e3f18b12bb89ee02ca7fdadb05ac1c1fd1
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441925"
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