---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a524c75e586d24f0f42e22ef6918482cd1222c642f568b83b3d9ec83781ba0b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156463"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const oAuth2PermissionGrant = {
  scope: 'scope-value'
};

await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .update(oAuth2PermissionGrant);

```