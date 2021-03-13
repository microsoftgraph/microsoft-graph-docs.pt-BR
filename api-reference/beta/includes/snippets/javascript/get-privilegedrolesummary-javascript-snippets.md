---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7003090174320283bd6400afd8c934ef0f0f9315
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806795"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let privilegedRoleSummary = await client.api('/privilegedRoles/{id}/summary')
    .version('beta')
    .get();

```