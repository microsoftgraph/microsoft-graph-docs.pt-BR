---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0c279a8e4f4d925ebecd820fd083e4d2642a47a8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780410"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/servicePrincipals/{id}/claimsMappingPolicies/$ref')
    .version('beta')
    .post(claimsMappingPolicy);

```