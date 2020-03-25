---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0f0b91d88bf41649f2a0290f5f456aca6f0f6d2
ms.sourcegitcommit: 33ffed5b785abf36b1a7786856c9266958830d25
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2020
ms.locfileid: "42947797"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const printUserIdentity = {
  @odata.id: "https://graph.microsoft.com/beta/users/{id}"
};

let res = await client.api('/print/printers/{id}/allowedUsers/$ref')
    .version('beta')
    .post(printUserIdentity);

```