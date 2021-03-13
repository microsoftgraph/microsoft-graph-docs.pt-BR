---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e106dd400aa301df6fac04271c00cf95b1892a11
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774682"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemAddress = {
  allowedAudiences: 'me',
  displayName: 'Secret Hideout',
};

await client.api('/users/{userId}/profile/addresses/{id}')
    .version('beta')
    .update(itemAddress);

```