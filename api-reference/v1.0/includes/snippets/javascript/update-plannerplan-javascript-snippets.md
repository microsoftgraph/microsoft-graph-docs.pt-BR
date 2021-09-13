---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8b3975dd77aafe47ccda502903677b224f764b54c96783c5fb2c253bc33f35e7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899504"
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