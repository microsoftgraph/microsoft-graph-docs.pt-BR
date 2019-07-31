---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a46e6ad60a5c16de0c2281c85bb2bd7fb30c570a
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730304"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerTask = {
  assignments: {
    fbab97d0-4932-4511-b675-204639209557: {
      @odata.type: "#microsoft.graph.plannerAssignment",
      orderHint: "N9917 U2883!"
    }
  },
  appliedCategories: {
    category3: true,
    category4: false
  }
};

let res = await client.api('/planner/tasks/01gzSlKkIUSUl6DF_EilrmQAKDhh')
    .version('beta')
    .update({plannerTask : plannerTask});

```