---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8891baf1951aea497fe746167834f23350eaf5a0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810071"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/names/{id}')
    .version('beta')
    .delete();

```