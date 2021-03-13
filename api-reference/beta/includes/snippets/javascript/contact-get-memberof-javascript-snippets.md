---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4303861f9f4c7b0f01366a65c388a439da5cf495
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792327"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let memberOf = await client.api('/contacts/{id}/memberOf')
    .version('beta')
    .get();

```