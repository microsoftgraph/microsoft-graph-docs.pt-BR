---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 10e3e5dbc4706161ff117e59be4d3ff93f575aa50afa2485aabfcea8306cd149
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213594"
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
    .version('beta')
    .post(reply);

```