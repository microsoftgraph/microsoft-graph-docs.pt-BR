---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12905d522928e3120adda1019ee4e8a63ff6d6e0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50785717"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let transitiveMemberOf = await client.api('/devices/{id}/transitiveMemberOf')
    .version('beta')
    .get();

```