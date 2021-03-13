---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbd35d2de39a9d8ecf18c5c1dd5f0082c37fa6b3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50783138"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/shares/{id}')
    .version('beta')
    .delete();

```