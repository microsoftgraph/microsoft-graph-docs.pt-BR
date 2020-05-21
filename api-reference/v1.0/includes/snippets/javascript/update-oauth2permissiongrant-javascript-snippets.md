---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd82cbb42f196234cb5f464623fe17587ac327cb
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335258"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  scope: "scope-value"
};

let res = await client.api('/oauth2PermissionGrants/{id}')
    .update(oAuth2PermissionGrant);

```