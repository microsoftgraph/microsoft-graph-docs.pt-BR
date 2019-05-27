---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2f633c2efc0effdf798c99710df31a26a20d8c0
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34440279"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: "2016-10-19T10:37:00Z",
  sentDateTime: "2016-10-19T10:37:00Z",
  hasAttachments: true,
  subject: "subject-value",
  body: {
    contentType: "",
    content: "content-value"
  },
  bodyPreview: "bodyPreview-value"
};

let res = await client.api('/me/mailFolders/{id}/messages')
    .version('beta')
    .post({message : message});

```