---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 306d3ea0e796e3a4d798e7468169a0b07d9e6c4d
ms.sourcegitcommit: 0329bbcd5f1b09a2a6c5f935a30c4560b6eed492
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/27/2019
ms.locfileid: "36636378"
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
    .update(plannerPlan);

```