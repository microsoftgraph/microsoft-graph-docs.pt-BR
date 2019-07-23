---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f42aa223c0dbbd9d912420baa1c5ad60246b740b
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35734343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const plannerPlan = {
  title: "title-value"
};

let res = await client.api('/planner/plans/{plan-id}')
    .update({plannerPlan : plannerPlan});

```