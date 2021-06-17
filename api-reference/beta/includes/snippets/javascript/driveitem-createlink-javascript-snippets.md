---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 08e6e8801162b5beac92946a430222d4048399e9
ms.sourcegitcommit: 979fe005c74eb99cd971df6b9511b2d3f7fe3cd4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "52990736"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const permission = {
  type: 'view',
  scope: 'anonymous',
  password: 'String',
  recipients: [
    {
      '@odata.type': 'microsoft.graph.driveRecipient'
    }
  ]
};

await client.api('/me/drive/items/{itemId}/createLink')
    .version('beta')
    .post(permission);

```