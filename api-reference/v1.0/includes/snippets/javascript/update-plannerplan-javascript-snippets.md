---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f984c9a47a0eafed08f3815db5c36769298365e8
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795527"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: 'title-value'
};

await client.api('/planner/plans/{plan-id}')
    .update(plannerPlan);

```