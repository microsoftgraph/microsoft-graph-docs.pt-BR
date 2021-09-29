---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8c95e0e28b7bf08cf1838ac1cfc343f30a4ba586
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59997188"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let getAttackSimulationTrainingUserCoverage = await client.api('/reports/getAttackSimulationTrainingUserCoverage')
    .version('beta')
    .get();

```