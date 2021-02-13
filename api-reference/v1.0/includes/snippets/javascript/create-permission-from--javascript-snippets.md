---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 563a1aa54a45156c39e5b1c58ac896e4266c95d4
ms.sourcegitcommit: 48fff935d56fe96e97577a80a3a0aa15c45419ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/10/2021
ms.locfileid: "50176767"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ["write"],
  grantedToIdentities: [{
    application: {
      id: "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      displayName: "Foo App"
    }
  }]
};

let res = await client.api('/sites/{sitesId}/permissions')
    .post(permission);

```