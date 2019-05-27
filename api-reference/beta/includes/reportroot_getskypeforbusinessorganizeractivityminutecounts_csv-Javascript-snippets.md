---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 88d52bb444e42b4a9255a199bbbfa0c056452dc8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464220"
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