---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b794727bd75fece787aebe70dce46e6f79aa1c6095f4193b7188b4243e5764ce
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327287"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/tokenIssuancePolicies/{id}')
    .version('beta')
    .update(tokenIssuancePolicy);

```