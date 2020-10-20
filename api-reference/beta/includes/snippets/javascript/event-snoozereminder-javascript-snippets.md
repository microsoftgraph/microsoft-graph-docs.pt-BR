---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13e68b69cb420ad9c1e1b9fa8926661e41a4f4f5
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48617698"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: "2016-10-19T10:37:00Z",
    timeZone: "timeZone-value"
  }
};

let res = await client.api('/me/events/{id}/snoozeReminder')
    .version('beta')
    .post(snoozeReminder);

```