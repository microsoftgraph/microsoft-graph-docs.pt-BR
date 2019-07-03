---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28d1a7d5e212209c25b316c7ac0f353d1ee06ffa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518028"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/plans/'id'')
    .version('beta')
    .get();

```