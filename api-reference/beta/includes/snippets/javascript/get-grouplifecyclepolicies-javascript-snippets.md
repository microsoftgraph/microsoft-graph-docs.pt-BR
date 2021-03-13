---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9afe2ee003c729fb84d1f81b7959000b6a5cbf0d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groupLifecyclePolicies = await client.api('/groups/{id}/groupLifecyclePolicies')
    .version('beta')
    .get();

```