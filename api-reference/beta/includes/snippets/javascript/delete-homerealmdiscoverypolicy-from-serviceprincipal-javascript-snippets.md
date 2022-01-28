---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 342c260c47b80592d377000a334acbbf39544c56673eec2d198db02fda9542be
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101953"
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