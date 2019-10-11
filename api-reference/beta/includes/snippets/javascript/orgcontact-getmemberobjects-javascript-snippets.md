---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1742bf6a2b866afa6bb4a591d5923d688fedc40
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428731"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

let res = await client.api('/contacts/{id}/getMemberObjects')
    .version('beta')
    .post(string);

```