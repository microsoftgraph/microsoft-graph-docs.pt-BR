---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 162cb9a64d7b81c52ee22d0ea77baee7e5653365c6aa058a614e8111fd45fb53
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272103"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: 'title-value'
};

await client.api('/planner/plans/{id}')
    .version('beta')
    .update(plannerPlan);

```