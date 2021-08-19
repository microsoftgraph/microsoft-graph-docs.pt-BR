---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee0b729046dde1a1ba16576b30eeb1231d6d4ddf9732cbee97ddb8d319b6efab
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156973"
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
  uid: 'iCalUId-value',
  reminderMinutesBeforeStart: 99,
  isReminderOn: true
};

await client.api('/groups/{id}/events/{id}')
    .version('beta')
    .update(event);

```