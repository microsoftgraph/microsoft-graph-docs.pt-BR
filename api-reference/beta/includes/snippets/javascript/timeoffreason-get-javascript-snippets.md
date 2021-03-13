---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0403a5c91b1e643fa0a81bab6748b6297ca818f9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50782531"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let timeOffReason = await client.api('/teams/{teamId}/schedule/timeOffReasons/{timeOffReasonId}')
    .version('beta')
    .get();

```