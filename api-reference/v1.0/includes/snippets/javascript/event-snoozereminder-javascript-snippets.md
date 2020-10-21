---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5c6c8e14db9c5c49c372ccabf622ef24c5a0c2f7
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606612"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: "dateTime-value",
    timeZone: "timeZone-value"
  }
};

let res = await client.api('/me/events/{id}/snoozeReminder')
    .post(snoozeReminder);

```