---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c80aa59134f1db93ec1334632d7de7522b11fab9
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42590032"
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
  isOrganizationDefault: true,
  type: "type-value"
};

let res = await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .update(homeRealmDiscoveryPolicy);

```