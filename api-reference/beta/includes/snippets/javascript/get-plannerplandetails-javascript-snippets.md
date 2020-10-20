---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f03a2e09b5285b55ac3de6a3e3ce8cf7069bbd20
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606781"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/xqQg5FS2LkCp935s-FIFm2QAFkHM/details')
    .version('beta')
    .get();

```