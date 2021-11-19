---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 298d9dfed9caeebbd2ea3b8701cdd58753d9c7e9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099289"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const externalItem = {
  acl: [
    {
      type: 'everyone',
      value: '67a141d8-cf4e-4528-ba07-bed21bfacd2d',
      accessType: 'grant',
    }
  ]
};

await client.api('/external/connections/contosohr/items/TSP228082938')
    .version('beta')
    .update(externalItem);

```