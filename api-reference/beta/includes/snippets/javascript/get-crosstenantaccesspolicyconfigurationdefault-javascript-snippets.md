---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c844f59e2a3b608d4a31028a8cd705de4663c9d5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let crossTenantAccessPolicyConfigurationDefault = await client.api('/policies/crossTenantAccessPolicy/default')
    .version('beta')
    .get();

```