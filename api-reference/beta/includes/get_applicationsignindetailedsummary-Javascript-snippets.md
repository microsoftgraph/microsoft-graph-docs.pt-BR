---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d888b3e604a5866af3029e5319b9dea1b53624b9
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34474020"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/reports/applicationSignInDetailedSummary/'id'')
    .version('beta')
    .get();

```