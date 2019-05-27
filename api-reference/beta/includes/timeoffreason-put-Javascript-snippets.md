---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0cfa06ed557aa66e0d43d4c57f917ef71ce108b3
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462124"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: "Vacation",
  iconType: "plane",
  isActive: true
};

let res = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .put({timeOffReason : timeOffReason});

```