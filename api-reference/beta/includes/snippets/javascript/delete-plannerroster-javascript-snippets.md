---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: aa61371532aeff4afb6e9ea0ccc8c9ce408d1df2
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271919"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/rosters/5ba84f7a-aa11-4a51-a298-9f2c7ec6bb38')
    .version('beta')
    .delete();

```