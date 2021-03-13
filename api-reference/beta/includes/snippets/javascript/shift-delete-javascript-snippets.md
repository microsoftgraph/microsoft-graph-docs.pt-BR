---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68410e6cb6e75fd9843709ca6be92cd47ad59472
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780053"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/shifts/{shiftId}')
    .version('beta')
    .delete();

```