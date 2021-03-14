---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4fffedfd9ef01cc22f2444adc9d81a8c37a5e02d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787088"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  receivedDateTime: 'datetime-value',
  sentDateTime: 'datetime-value',
  hasAttachments: true,
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  bodyPreview: 'bodyPreview-value'
};

await client.api('/me/mailFolders/{id}/messages')
    .post(message);

```