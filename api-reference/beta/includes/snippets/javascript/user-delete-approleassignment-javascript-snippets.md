---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5baf37ae3467583ceef313089611e41959a6dbbb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809525"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{id}/appRoleAssignments/{id}')
    .version('beta')
    .delete();

```