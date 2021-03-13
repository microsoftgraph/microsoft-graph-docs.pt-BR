---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5100272574d005cb5e4bd6d5ff6538f0cba61a62
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50799264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/me/profile/websites/{id}')
    .version('beta')
    .delete();

```