---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39f6428a9009f12822686cb225db54d5ccac28e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803753"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/jobs/{id}/abort')
    .version('beta')
    .post();

```