---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 940086dbdef0967f468846d489ab5662161a62d2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518189"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/auditLogs/directoryAudits')
    .version('beta')
    .get();

```