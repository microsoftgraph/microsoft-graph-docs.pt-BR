---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1a9ad177b377100dac687dbb0f0722919a6e818f115bd19bdb60ad1426fb59b2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099671"
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