---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3ab43eae2ab6a82e98ba65f29188b3023692379
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774486"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let printTaskTrigger = await client.api('/print/printers/{printerId}/taskTriggers/{printTaskTriggerId}')
    .get();

```