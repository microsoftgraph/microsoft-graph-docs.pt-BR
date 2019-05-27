---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4422cdaa8c09156f435ad13db6bdbea98c1d9241
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34463810"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```