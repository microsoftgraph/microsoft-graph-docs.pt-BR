---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e8ebd9b67a9289a75ee4b8dd86703a5f7459310c
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  originalStartTimeZone: "originalStartTimeZone-value",
  originalEndTimeZone: "originalEndTimeZone-value",
  responseStatus: {
    response: "",
    time: "datetime-value"
  },
  recurrence: null,
  iCalUId: "iCalUId-value",
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

let res = await client.api('/me/events/{id}')
    .update({event : event});

```