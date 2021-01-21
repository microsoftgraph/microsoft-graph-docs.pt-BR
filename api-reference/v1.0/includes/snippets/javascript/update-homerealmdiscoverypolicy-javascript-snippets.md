---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7940f7025bcbff070ed70ef26638f55ab701e94d
ms.sourcegitcommit: 6314172db76ba9f2c192d8c099d818c5e772d2b8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2021
ms.locfileid: "49910392"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .update(homeRealmDiscoveryPolicy);

```