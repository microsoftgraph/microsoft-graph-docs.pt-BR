---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44481a6dea977455fdec749be9be1252199e9230
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801805"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: '2016-10-19T10:37:00Z',
  sentDateTime: '2016-10-19T10:37:00Z',
  hasAttachments: true,
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  bodyPreview: 'bodyPreview-value'
};

await client.api('/me/mailFolders/{id}/messages')
    .version('beta')
    .post(message);

```