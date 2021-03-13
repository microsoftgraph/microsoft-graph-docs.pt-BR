---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 64beac6d7667a117a84c1fd729b7f61ddc33d1ad
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795729"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/privilegedRoleAssignments/{id}')
    .version('beta')
    .delete();

```