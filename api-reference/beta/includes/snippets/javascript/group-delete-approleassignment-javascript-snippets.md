---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ce128b00cbb9c684424793c7241024dff9743cf1
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333168"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```