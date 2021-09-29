---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35c173208833975d9ba049c8312402459d2a00b6
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59996513"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAttackSimulationRepeatOffenders = await client.api('/reports/getAttackSimulationRepeatOffenders')
    .version('beta')
    .get();

```