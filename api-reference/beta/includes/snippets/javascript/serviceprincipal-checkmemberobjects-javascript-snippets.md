---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4398f1871fcb5fddef105a8f94c2c247390fce96
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428744"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  ids: [
    "80a963dd-84af-4eb8-b2a6-781e444d4fb0",
    "62e90394-69f5-4237-9190-012177145e10",
    "86a64f51-3a64-4cc6-a8c8-6b8f000c0f52",
    "ac38546e-ddf3-437a-ac5c-27a94cd7a0f1"
  ]
};

let res = await client.api('/servicePrincipals/{id}/checkMemberObjects')
    .version('beta')
    .post(string);

```