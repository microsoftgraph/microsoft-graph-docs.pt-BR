---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dfb6528f1ae31f440994ff66b96aae24eb07da6d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519478"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessOrganizerActivityCounts(period='D7')')
    .version('beta')
    .get();

```