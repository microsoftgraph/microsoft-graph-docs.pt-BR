---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6aef214b36397ab4371db0175aa2398d1de759d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498257"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/directReports')
    .version('beta')
    .get();

```