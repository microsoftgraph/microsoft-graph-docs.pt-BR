---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a18cc472fa64462575ea558d995c905dda5844d18547e56d0a1c330609e8fe8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102739"
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

await client.api('/policies/tokenIssuancePolicies')
    .post(tokenIssuancePolicy);

```