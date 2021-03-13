---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c38392feb1517e776e19430af49664fb4a0d84be
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskTrigger = await client.api('/print/printers/{printerId}/taskTriggers/{taskTriggerId}')
    .version('beta')
    .get();

```