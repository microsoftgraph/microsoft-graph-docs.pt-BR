---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d7da81a03d32006e263b42101b2c79c7c3c908f18df406eb09a77867d9cc50a3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159008"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: 'Let\'s go for lunch',
  body: {
    contentType: 'HTML',
    content: 'Does next month work for you?'
  },
  start: {
      dateTime: '2019-03-10T12:00:00',
      timeZone: 'Pacific Standard Time'
  },
  end: {
      dateTime: '2019-03-10T14:00:00',
      timeZone: 'Pacific Standard Time'
  },
  location: {
      displayName: 'Harry\'s Bar'
  },
  attendees: [
    {
      emailAddress: {
        address: 'adelev@contoso.onmicrosoft.com',
        name: 'Adele Vance'
      },
      type: 'required'
    }
  ],
  isOnlineMeeting: true,
  onlineMeetingProvider: 'teamsForBusiness'
};

await client.api('/me/calendars/AAMkAGViNDU9zAAAAAGtlAAA=/events')
    .post(event);

```