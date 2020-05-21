---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7d601eae0a950122e0d82ab573460bf4133bf27
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774762"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendarPermission = {
  role: "write"
};

let res = await client.api('/users/AlexW@contoso.OnMicrosoft.com/calendars/AAMkADAwAABf02bAAAA=/calendarPermissions/L289RXhjaGFuZ2VMYWJQWRlbGVW')
    .version('beta')
    .update(calendarPermission);

```