---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed964a8287a2f6b532b8c847e9c357c7b5e83703
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809968"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/teams/{teamId}/schedule/timesOff/{timeOffId}')
    .version('beta')
    .delete();

```