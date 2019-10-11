---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da8ef65118542467774465579d40d6a446347be1
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428747"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  groupIds: [
    "groupIds-value"
  ]
};

let res = await client.api('/servicePrincipals/{id}/checkMemberGroups')
    .version('beta')
    .post(string);

```