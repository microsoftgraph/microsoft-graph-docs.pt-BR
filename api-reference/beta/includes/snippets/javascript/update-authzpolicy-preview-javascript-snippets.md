---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27097504265ff9012fdd1c84a55c58ea7539b19c
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/02/2020
ms.locfileid: "47842873"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authorizationPolicy = {
  enabledPreviewFeatures: ["assignGroupsToRoles"]
};

let res = await client.api('/policies/authorizationPolicy/authorizationPolicy')
    .version('beta')
    .update(authorizationPolicy);

```