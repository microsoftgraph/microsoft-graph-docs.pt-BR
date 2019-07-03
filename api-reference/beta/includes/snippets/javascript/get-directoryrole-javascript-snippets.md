---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 512bd57f245ec1a01fbaea3916138b645d865d73
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518183"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/directoryRoles/{id}')
    .version('beta')
    .get();

```