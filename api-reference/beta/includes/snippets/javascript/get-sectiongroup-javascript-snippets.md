---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5341f88326a350423c94835c6a474f90927a20fa
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476448"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/sectionGroups/{id}')
    .version('beta')
    .get();

```