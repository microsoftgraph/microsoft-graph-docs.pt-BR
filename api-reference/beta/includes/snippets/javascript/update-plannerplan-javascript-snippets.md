---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bddebd3ebb8600ca259c102281a063e74d5658ab
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35720504"
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