---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecfa56910f88800650e6a8e80502b0496433f568
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/05/2021
ms.locfileid: "49753551"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const calendar = {
  name: "Marketing calendar"
};

let res = await client.api('/me/calendargroups/AAMkADYAAAR9NR5AAA=/calendars')
    .version('beta')
    .post(calendar);

```