---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39222b810ce66e719ff62953c2e432a9c239d64e
ms.sourcegitcommit: 1585d55d3e7030b5fd1f7cfd5de8f9fb8202cd56
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2019
ms.locfileid: "37428768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: false
};

let res = await client.api('/groups/{id}/getMemberObjects')
    .post(string);

```