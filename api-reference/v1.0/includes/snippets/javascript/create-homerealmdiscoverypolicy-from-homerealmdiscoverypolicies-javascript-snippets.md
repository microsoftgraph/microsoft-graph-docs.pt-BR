---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: acf0416f69de587c651759b13d66c1cb32e59796
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62351346"
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
    displayName: 'displayName-value',
    isOrganizationDefault: true
};

await client.api('/policies/homeRealmDiscoveryPolicies')
    .post(homeRealmDiscoveryPolicy);

```