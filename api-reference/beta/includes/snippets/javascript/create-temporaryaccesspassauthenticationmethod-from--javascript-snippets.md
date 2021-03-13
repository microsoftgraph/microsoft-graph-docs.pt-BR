---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a564f506a4527f599e98840d389b85682df89bd7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788337"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const temporaryAccessPassAuthenticationMethod = {
  '@odata.type': '#microsoft.graph.temporaryAccessPassAuthenticationMethod',
  startDateTime: '2021-01-26T00:00:00.000Z',
  lifetimeInMinutes: 60,
  isUsableOnce: false
};

await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods')
    .version('beta')
    .post(temporaryAccessPassAuthenticationMethod);

```