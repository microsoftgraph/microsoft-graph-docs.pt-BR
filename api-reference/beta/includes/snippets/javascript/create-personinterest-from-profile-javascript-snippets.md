---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53b994e1bae756c435abe95e1479bdd99b2fb57e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778146"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personInterest = {
  categories: [
    'Sports'
  ],
  description: 'World\'s greatest football club',
  displayName: 'Chelsea FC',
  webUrl: 'https://www.chelseafc.com'
};

await client.api('/me/profile/interests')
    .version('beta')
    .post(personInterest);

```