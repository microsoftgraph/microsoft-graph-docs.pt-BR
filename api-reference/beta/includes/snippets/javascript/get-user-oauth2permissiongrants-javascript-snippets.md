---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 908bbaf56621e6a6b30ccacdc99cfe3296b7f61b
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332550"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/users/{id}/oauth2PermissionGrants')
    .version('beta')
    .get();

```