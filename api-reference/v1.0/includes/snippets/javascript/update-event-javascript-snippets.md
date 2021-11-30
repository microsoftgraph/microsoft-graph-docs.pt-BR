---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43c30135907e30b43abd8c84b6df77ae4a33e27e
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61228311"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  originalStartTimeZone: 'originalStartTimeZone-value',
  originalEndTimeZone: 'originalEndTimeZone-value',
  responseStatus: {
    response: '',
    time: 'datetime-value'
  },
  recurrence: null,
  reminderMinutesBeforeStart: 99,
  isOnlineMeeting: true,
  onlineMeetingProvider: 'teamsForBusiness',
  isReminderOn: true,
  hideAttendees: false,
  categories: ['Red category']
};

await client.api('/me/events/{id}')
    .update(event);

```