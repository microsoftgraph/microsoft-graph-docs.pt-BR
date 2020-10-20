---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5f35c328a415de6839e85ffa44f41302c9c26edf
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48615500"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const onenoteOperation = {
  id: "id-value",
  groupId: "groupId-value"
};

let res = await client.api('/me/onenote/pages/{id}/copyToSection')
    .version('beta')
    .post(onenoteOperation);

```