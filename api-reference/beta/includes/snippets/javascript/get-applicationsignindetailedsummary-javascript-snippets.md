---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d888b3e604a5866af3029e5319b9dea1b53624b9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35710199"
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