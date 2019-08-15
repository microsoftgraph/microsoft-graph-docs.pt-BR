---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6010dcba86224473906635da661e7ff93a2d5721
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413676"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  recipients: [
    {
      email: "john@contoso.com"
    },
    {
      email: "ryan@external.com"
    }
  ],
  roles: ["read"]
};

let res = await client.api('/shares/{encoded-sharing-url}/permission/grant')
    .version('beta')
    .post(permission);

```