---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ff7c94660bfd3b71e2e68e320c5cd49f420fc474
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774338"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const itemEmail = {
  displayName: 'Business Email',
  type: 'work'
};

await client.api('/users/{userId}/profile/emails/{id}')
    .version('beta')
    .update(itemEmail);

```