---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d43dd9f7cda1eb83c25522c715a3d2ab42d5ce5d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791955"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const message = {
  subject: 'subject-value',
  body: {
    contentType: '',
    content: 'content-value'
  },
  inferenceClassification: 'other'
};

await client.api('/me/messages/{id}')
    .version('beta')
    .update(message);

```