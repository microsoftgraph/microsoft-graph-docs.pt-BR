---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64cf9529c2b7dc966a01e81d74e58c6ec1495822
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50800335"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```