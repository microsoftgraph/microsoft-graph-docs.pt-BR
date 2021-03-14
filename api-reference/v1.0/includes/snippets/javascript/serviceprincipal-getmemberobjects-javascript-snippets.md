---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a34c81c8dceb00a1899291654531310ef31715e4
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792769"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const string = {
  securityEnabledOnly: true
};

await client.api('/servicePrincipals/{id}/getMemberObjects')
    .post(string);

```