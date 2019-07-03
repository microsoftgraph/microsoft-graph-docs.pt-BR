---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88d52bb444e42b4a9255a199bbbfa0c056452dc8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518768"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityMinuteCounts(period='D7')')
    .version('beta')
    .get();

```