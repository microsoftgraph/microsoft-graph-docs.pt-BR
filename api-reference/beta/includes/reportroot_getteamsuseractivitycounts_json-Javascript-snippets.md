---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44c752f47a707484314f3cfa8b4a546dd6ffdc34
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462933"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getTeamsUserActivityCounts(period='D7')')
    .version('beta')
    .get();

```