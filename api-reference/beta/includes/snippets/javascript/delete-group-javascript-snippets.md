---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d25e6272ffe0ac127b1a839568146d12d812a79b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780135"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/groups/{id}')
    .version('beta')
    .delete();

```