---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0ba555704798629df7eb0110a5d3b7f039f59e9c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788079"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let groups = await client.api('/termStore/groups')
    .version('beta')
    .get();

```