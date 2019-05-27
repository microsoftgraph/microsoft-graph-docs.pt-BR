---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3c9b244ecfe46d3ab05a481358e527473fe37c6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441630"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getOffice365ActiveUserCounts(period='D7')')
    .version('beta')
    .get();

```