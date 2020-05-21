---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb2d19c1897e8e9885581f4e6076a30516e7f761
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333018"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/appRoleAssignments')
    .version('beta')
    .get();

```