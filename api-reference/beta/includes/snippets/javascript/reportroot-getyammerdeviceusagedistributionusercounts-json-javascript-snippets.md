---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cedf0d8ef9638eb065d7ba720949f14c943ebeed
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35718454"
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