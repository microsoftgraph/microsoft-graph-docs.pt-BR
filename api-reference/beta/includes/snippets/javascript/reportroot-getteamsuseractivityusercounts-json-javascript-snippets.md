---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 881eb3215da3503ded16cd0e12c004d6cc3c763d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35477343"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```