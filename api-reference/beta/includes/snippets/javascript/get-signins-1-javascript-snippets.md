---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5c4630d87c26460928951f672444cb37ac38f03
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805859"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let signIns = await client.api('/auditLogs/signIns')
    .version('beta')
    .get();

```