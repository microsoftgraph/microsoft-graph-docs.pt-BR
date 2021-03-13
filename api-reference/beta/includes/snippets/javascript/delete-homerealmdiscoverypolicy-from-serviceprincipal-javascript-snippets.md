---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cb7310bb66a2a5b856938dc65b9204f0fe6a6400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787659"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref')
    .version('beta')
    .delete();

```