---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 38ed024c5db1331a153d358bab5952daa5b09e09
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48614027"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskGroups')
    .version('beta')
    .get();

```