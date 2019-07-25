---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19409310cc3b55809494bf311405f5e34df8d7d2
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35709171"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const event = {
  subject: "Let's go for lunch",
  body: {
    contentType: "HTML",
    content: "Does next month work for you?"
  },
  start: {
      dateTime: "2019-03-10T12:00:00",
      timeZone: "Pacific Standard Time"
  },
  end: {
      dateTime: "2019-03-10T14:00:00",
      timeZone: "Pacific Standard Time"
  },
  location:{
      displayName:"Harry's Bar"
  },
  attendees: [
    {
      emailAddress: {
        address:"adelev@contoso.onmicrosoft.com",
        name: "Adele Vance"
      },
      type: "required"
    }
  ]
};

let res = await client.api('/me/calendars/AAMkAGViNDU7zAAAAAGtlAAA=/events')
    .version('beta')
    .post({event : event});

```