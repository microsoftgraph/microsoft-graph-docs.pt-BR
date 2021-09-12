---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44d125ea2e9b2569fe8b64e31cca74d971e8896dbf1bb05a8876da798ace8013
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100625"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let plannerPlanDetails = await client.api('/planner/plans/{plan-id}/details')
    .get();

```