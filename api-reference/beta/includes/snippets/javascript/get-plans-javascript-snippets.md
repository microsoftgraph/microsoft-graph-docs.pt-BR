---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 551da0259c67eced0dad5ea40875c573b00584a9
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519267"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/planner/plans')
    .version('beta')
    .get();

```