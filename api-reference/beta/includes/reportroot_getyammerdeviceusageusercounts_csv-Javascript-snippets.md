---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bef00660b19542d04996732bc59e4a5b5badcf2f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482049"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserCounts(period='D7')')
    .version('beta')
    .get();

```