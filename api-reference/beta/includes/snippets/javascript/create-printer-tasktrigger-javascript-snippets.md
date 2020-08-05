---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dede494aba117d9f9d82a01365c876f9a2dde259
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46565863"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printTaskTrigger = {
  event: "jobStarted",
  definition@odata.bind: "https://graph.microsoft.com/beta/print/taskDefinitions/3203656e-6069-4e10-8147-d25290b00a3c"
};

let res = await client.api('/print/printers/ae63f617-4856-4b45-8ea9-69dfbeea230e/taskTriggers')
    .version('beta')
    .post(printTaskTrigger);

```