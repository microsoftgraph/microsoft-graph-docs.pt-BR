---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 60861157b35ed82f6626f82815cee65f19e0dee7
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787944"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let certificateBasedAuthConfiguration = await client.api('/organization/{id}/certificateBasedAuthConfiguration')
    .version('beta')
    .get();

```