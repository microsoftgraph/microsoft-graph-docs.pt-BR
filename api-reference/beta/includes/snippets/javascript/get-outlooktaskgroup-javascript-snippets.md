---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f5e0e68867fe04fd7b7d20d1d169eb3a585c913
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777953"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let outlookTaskGroup = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .get();

```