---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 527375752d2efed1d13e2d8613d8dddac0754c83
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428739"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/me/getMemberGroups')
    .version('beta')
    .post(string);

```