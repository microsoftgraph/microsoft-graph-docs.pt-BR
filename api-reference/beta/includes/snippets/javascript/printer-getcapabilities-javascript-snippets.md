---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cfce0ce14e8eadff6593e3d4ac32a4bb39f07ebc
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947972"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/getCapabilities')
    .version('beta')
    .post();

```