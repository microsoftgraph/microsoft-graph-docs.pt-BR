---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70660ba52ff51d645d723d3287448f172a586ddf
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808460"
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