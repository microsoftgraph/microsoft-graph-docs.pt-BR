---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4536113de7897565e8cd704e1bf9fe16fbd1b93
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786971"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    'groupIds-value'
  ]
};

await client.api('/groups/{id}/checkMemberGroups')
    .version('beta')
    .post(string);

```