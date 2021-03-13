---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 30f55e070a2b0a4cac7cbebd040a2ca7cc9cad61
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772608"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let estimateStatisticsOperation = await client.api('/compliance/ediscovery/cases/{caseId}/sourceCollections/95bdbf84f02f4bdaafbbb2fe945a4962/lastEstimateStatisticsOperation')
    .version('beta')
    .get();

```