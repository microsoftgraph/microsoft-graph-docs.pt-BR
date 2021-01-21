---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 47e0ba2ac8a2e3c1c486ffbe16074b57c0dfecc5
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910321"
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
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenLifetimePolicies/{id}')
    .update(tokenLifetimePolicy);

```