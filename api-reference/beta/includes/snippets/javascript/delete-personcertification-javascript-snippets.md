---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3393248f825b6c7669024eebca4247313711bf7b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774058"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/users/{userId}/profile/certifications/{id}')
    .version('beta')
    .delete();

```