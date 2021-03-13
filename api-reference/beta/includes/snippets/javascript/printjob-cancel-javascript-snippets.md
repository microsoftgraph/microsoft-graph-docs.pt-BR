---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c91d69eca4ae519717d30272697aeb131dd25d3f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805688"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/print/printers/{id}/jobs/{id}/cancel')
    .version('beta')
    .post();

```