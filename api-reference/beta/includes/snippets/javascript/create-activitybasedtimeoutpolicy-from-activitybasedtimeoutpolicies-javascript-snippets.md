---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 907327739d8b5f9d4ee89ed95312b90d322b9eb1
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475424"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const policy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .post(policy);

```