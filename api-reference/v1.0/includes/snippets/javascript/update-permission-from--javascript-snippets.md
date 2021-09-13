---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e61dcf15749122d5eb817692b2d78d51c9808538f925b1afda6ef789c7563e47
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56897732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  roles: ['read']
};

await client.api('/sites/{sitesId}/permissions/{permissionId}')
    .update(permission);

```