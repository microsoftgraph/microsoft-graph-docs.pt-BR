---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ffe91672dc2e6e20e9c71974274dbec6e27b3f0e
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50798575"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/devices/{id}/registeredOwners/{id}/$ref')
    .version('beta')
    .delete();

```