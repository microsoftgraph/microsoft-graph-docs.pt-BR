---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd487535937e65e3178ca297cb3a4ee0ead4e8dc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802082"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const timeOffReason = {
  displayName: 'Vacation',
  iconType: 'plane',
  isActive: true
};

await client.api('/teams/{teamId}/schedule/timeOffReasons')
    .version('beta')
    .post(timeOffReason);

```