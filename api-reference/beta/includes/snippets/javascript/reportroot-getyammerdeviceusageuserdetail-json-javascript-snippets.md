---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06f8c4ac11665a9d7e5e03e696d3472e18a83b39
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498239"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getYammerDeviceUsageUserDetail(period='D7')')
    .version('beta')
    .get();

```