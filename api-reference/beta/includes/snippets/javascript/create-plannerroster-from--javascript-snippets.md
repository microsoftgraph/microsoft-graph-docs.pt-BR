---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 55a3cbca148bdabe8abe382a3bbd700c1ef64713
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50272001"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerRoster = {
  @odata.type: "#microsoft.graph.plannerRoster"
};

let res = await client.api('/planner/rosters')
    .version('beta')
    .post(plannerRoster);

```