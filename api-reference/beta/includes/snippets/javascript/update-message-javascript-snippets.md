---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: abc0955b29e2beb81d5c3dd67928ce367b2e451e13e499989cd3644a84a58d25
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213702"
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