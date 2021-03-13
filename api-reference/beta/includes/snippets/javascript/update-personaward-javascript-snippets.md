---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 565d0eb1fbf0dc39d6d17713a245214506b8452e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774100"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const personAward = {
  issuingAuthority: 'International Association of Branding Management',
  thumbnailUrl: 'https://iabm.io/sdhdfhsdhshsd.jpg'
};

await client.api('/users/{userId}/profile/awards/{personAwardId}')
    .version('beta')
    .update(personAward);

```