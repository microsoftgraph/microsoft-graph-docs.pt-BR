---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6e65d7f2cfa53b1dc7d66bab11cba5bb22594c2
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664508"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationContextClassReference = {
   value: 
    [
      {
         displayName: 'Contoso trusted locations',
        description: 'Access is only allowed from trusted locations',
        isAvailable: true
      }
    ]
};

await client.api('/identity/conditionalAccess/authenticationContextClassReferences/c1')
    .version('beta')
    .update(authenticationContextClassReference);

```