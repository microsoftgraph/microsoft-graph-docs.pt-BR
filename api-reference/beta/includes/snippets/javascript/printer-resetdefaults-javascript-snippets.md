---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1ac1d4ef26303ac3c814b6cac1168c92b070540
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/resetDefaults')
    .version('beta')
    .post();

```