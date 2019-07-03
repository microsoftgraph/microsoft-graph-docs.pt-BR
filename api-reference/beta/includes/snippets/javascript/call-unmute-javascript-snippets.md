---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 268b8c52bab21f2f238d0d4ceb8c3af54d996e58
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518716"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "clientContext-value"
};

let res = await client.api('/app/calls/{id}/unmute')
    .version('beta')
    .post(CommsOperation);

```