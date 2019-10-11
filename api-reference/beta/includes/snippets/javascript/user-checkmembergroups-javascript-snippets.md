---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d1c60b70048f84ea604a1c72556c7f1205f51d84
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428689"
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

let res = await client.api('/me/checkMemberGroups')
    .version('beta')
    .post(string);

```