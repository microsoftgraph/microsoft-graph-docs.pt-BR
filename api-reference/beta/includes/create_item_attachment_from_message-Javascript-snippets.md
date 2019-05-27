---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a57fe33fe3c67d127c3fc194504ba583cbeede37
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const attachment = {
  @odata.type: "#microsoft.graph.itemAttachment",
  name: "Holiday event", 
  item: {
    @odata.type: "microsoft.graph.event",
    subject: "Discuss gifts for children",
    body: {
      contentType: "HTML",
      content: "Let's look for funding!"
    },
    start: {
      dateTime: "2016-12-02T18:00:00",
      timeZone: "Pacific Standard Time"
    },
    end: {
      dateTime: "2016-12-02T19:00:00",
      timeZone: "Pacific Standard Time"
    }
  }
};

let res = await client.api('/me/messages/AAMkpsDRVK/attachments')
    .version('beta')
    .post({attachment : attachment});

```