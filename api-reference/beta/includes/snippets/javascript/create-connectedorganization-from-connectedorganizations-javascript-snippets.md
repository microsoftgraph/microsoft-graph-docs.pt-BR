---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f1c9ae71507d9e2c6206dab8d757d74640e99a39
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566529"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const connectedOrganization = {
  displayName:"Connected organization name",
  description:"Connected organization description",
  identitySources: [
    {
      @odata.type: "#microsoft.graph.domainIdentitySource",
      domainName: "example.com",
      displayName: "example.com"
      }
  ]
};

let res = await client.api('/identityGovernance/entitlementManagement/connectedOrganizations/')
    .version('beta')
    .post(connectedOrganization);

```