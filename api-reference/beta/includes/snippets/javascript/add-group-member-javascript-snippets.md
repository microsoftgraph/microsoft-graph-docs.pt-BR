---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8118d35fb86502260e1dede246a9b475232cc836
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783221"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const directoryObject = {
  '@odata.id': 'https://graph.microsoft.com/beta/directoryObjects/{id}'
};

await client.api('/groups/{group-id}/members/$ref')
    .version('beta')
    .post(directoryObject);

```