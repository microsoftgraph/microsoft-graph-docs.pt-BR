---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31db1d41d6357756d7baf71b689d72cd46077dd7
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994481"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: "user",
      value: "49103559-feac-4575-8b94-254814dfca72",
      accessType: "grant",
      identitySource: "Azure Active Directory"
    }
  ]
};

let res = await client.api('/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```