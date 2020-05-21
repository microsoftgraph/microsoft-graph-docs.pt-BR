---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8513b78d068a9eabfc7d5ea43ec547b432f10f61
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44332396"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/groups/{id}/appRoleAssignments/{id}')
    .delete();

```