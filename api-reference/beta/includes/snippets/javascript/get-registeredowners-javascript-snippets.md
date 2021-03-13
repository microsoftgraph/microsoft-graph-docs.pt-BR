---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 580c49093fad3220865be0f7558f972b7243dadb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804315"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let registeredOwners = await client.api('/devices/{id}/registeredOwners')
    .version('beta')
    .get();

```