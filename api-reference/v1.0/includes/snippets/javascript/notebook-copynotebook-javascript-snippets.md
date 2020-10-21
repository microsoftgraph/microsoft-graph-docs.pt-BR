---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e02e3b60a0fbec2cdf628830ee628a46fcffd94
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606411"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  groupId: "groupId-value",
  renameAs: "renameAs-value"
};

let res = await client.api('/me/onenote/notebooks/{id}/copyNotebook')
    .post(onenoteOperation);

```