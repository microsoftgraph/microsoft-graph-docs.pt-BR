---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4522a0023aa71d878bcf30c38626898dd5216d50
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464528"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/getSkypeForBusinessActivityUserCounts(period='D7')')
    .version('beta')
    .get();

```