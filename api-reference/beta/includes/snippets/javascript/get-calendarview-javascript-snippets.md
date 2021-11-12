---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bc9649fbba5dbec96cef2013bc7f36ebeaddb75f80baf2edfe336ecfe63479bc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102548"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let calendarView = await client.api('/me/calendar/calendarView?startDateTime=2017-01-01T19:00:00-08:00&endDateTime=2017-01-07T19:00:00-08:00')
    .version('beta')
    .get();

```