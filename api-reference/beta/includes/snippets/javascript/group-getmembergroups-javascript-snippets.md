---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c144216cc5c0487cb3dfec794b97aac481805099
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428723"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberGroups')
    .version('beta')
    .post(string);

```