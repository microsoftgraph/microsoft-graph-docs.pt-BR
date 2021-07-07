---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53edb31258bb8338cd3bebc3d5abf1f6fac91795
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319544"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let rules = await client.api('/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules')
    .version('beta')
    .get();

```