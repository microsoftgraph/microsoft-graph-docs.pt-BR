---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b261864db62a37309b209598f6c9cf9ebee01700
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795123"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const snoozeReminder = {
  newReminderTime: {
    dateTime: '2016-10-19T10:37:00Z',
    timeZone: 'timeZone-value'
  }
};

await client.api('/me/events/{id}/snoozeReminder')
    .version('beta')
    .post(snoozeReminder);

```