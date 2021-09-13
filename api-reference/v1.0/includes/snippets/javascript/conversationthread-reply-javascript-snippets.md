---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a539ea1d97c6bec65e2aa057850894f82beffbd00d031ec62db329ab8a7c167
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272925"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const reply = {
  post: {
    body: {
      contentType: '',
      content: 'content-value'
    }
  }
};

await client.api('/groups/{id}/threads/{id}/reply')
    .post(reply);

```