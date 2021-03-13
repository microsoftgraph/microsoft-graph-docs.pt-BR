---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9ef36037f28f4ab43fd779b3a3b061fb9ccbe37b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50796308"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const conversationThread = {
  originalStartTimeZone: 'originalStartTimeZone-value',
  originalEndTimeZone: 'originalEndTimeZone-value',
  responseStatus: {
    response: '',
    time: 'datetime-value'
  },
  uid: 'iCalUId-value',
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

await client.api('/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/threads/AAQkAGI5MWY5ZmUyLTJiNzYtNDE0ZC04OWEwLWM3M2FjYmM3NzNlZgMkABAAG5c7eC4NYEynIoXsuxXB9RAAG5c7eC4NYEynIoXsuxXB9Q==')
    .version('beta')
    .update(conversationThread);

```