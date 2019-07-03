---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cedf0d8ef9638eb065d7ba720949f14c943ebeed
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476336"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```