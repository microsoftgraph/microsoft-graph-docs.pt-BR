---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 797cd205e0d27039f49b16bccc74d24ec15c9417
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207349"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicyAssignments = await client.api('/policies/roleManagementPolicyAssignments')
    .filter('scopeId eq \'/\' and scopeType eq \'Directory\'')
    .get();

```