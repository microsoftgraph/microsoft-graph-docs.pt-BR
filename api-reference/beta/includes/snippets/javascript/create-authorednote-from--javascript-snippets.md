---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8c4e0a23b393ea64ebc3afe6d8120a3df4a9d88
ms.sourcegitcommit: 0eb843a6f61f384bc28c0cce1ccb74f64bdb1fa6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/23/2021
ms.locfileid: "60561833"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authoredNote = {
content: 
  {
    content: 'String',
    contentType: 'text'
  }
};

await client.api('/privacy/subjectRightsRequests/{subjectRightsRequestId}/notes')
    .version('beta')
    .post(authoredNote);

```