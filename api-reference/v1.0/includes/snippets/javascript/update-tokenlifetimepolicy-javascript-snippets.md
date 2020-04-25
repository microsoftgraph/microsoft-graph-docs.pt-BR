---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32201c8c20a303d4543716b4dc104b8bc6b12ec8
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806026"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenLifetimePolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true,
  type: "type-value"
};

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .update(tokenLifetimePolicy);

```