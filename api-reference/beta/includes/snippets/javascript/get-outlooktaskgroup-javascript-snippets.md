---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ecd5f1a44578abdb95379dbe09c4746f7c15ca9a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518989"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/outlook/taskGroups/AAMkADIyAAAhrbe-AAA=')
    .version('beta')
    .get();

```