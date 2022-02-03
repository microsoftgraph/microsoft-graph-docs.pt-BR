---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c693f431410fd7661c8ae3d4d667abf0d197d96
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351811"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
    definition: [
    '{\"HomeRealmDiscoveryPolicy\':
     {\'AccelerateToFederatedDomain\':true,
      \'PreferredDomain\':\"federated.example.edu\",
      \'AlternateIdLogin\':{\'Enabled\':true}}}"
  ],
    displayName: 'Contoso default HRD Policy'
};

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .version('beta')
    .update(homeRealmDiscoveryPolicy);

```