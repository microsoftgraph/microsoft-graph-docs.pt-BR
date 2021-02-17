---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89790af61558f0848c1c0ac04a4773e87fa4a58d
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50271882"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/planner/rosters/6519868f-868f-6519-8f86-19658f861965')
    .version('beta')
    .get();

```