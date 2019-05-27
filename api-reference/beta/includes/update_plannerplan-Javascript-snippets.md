---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bddebd3ebb8600ca259c102281a063e74d5658ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464966"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: "title-value"
};

let res = await client.api('/planner/plans/'id'')
    .version('beta')
    .update({plannerPlan : plannerPlan});

```