---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bef00660b19542d04996732bc59e4a5b5badcf2f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35726313"
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