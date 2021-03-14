---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 288a495249b62aa0a0173d64eef125e5c0687eb3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50781789"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlan = await client.api('/planner/plans/{plan-id}')
    .get();

```