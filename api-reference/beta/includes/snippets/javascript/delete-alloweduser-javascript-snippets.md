---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1888ec40f1f3a8588b90b96a2e39ab2f2962433d
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42948056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/print/printers/{id}/allowedUsers/{id}/$ref')
    .version('beta')
    .delete();

```