---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbce78d1b149c2296739423e2aac2b56ec797d58
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/restoreFactoryDefaults')
    .version('beta')
    .post();

```