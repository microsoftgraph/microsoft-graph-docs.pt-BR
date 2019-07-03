---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6dc46ec8201f3f041debd7de87e221e6aa255c64
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519127"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessDeviceUsageDistributionUserCounts(period='D7')')
    .version('beta')
    .get();

```