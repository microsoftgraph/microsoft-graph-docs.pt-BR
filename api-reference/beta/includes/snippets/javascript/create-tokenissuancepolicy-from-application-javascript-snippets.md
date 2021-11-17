---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c131b4168e14ab41aae95f2e3468ee0193840b32a77f8537669c67179ddf5eea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156836"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/tokenIssuancePolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/applications/{id}/tokenIssuancePolicies/$ref')
    .version('beta')
    .post(tokenIssuancePolicy);

```