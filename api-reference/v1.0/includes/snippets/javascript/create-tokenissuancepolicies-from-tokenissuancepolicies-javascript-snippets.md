---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5cb87c8cf7a2a4f245235004f8844ccc4c6bc70
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805353"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tokenIssuancePolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true
};

let res = await client.api('/policies/tokenIssuancePolicies')
    .post(tokenIssuancePolicy);

```