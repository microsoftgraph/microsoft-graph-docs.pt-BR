---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9563578dab2484381d056e1ba15780dc4acd2fb590a024fd4c89b98fe38901b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272843"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let oAuth2PermissionGrant = await client.api('/oauth2PermissionGrants/{id}')
    .version('beta')
    .get();

```