---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 940086dbdef0967f468846d489ab5662161a62d2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472108"
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