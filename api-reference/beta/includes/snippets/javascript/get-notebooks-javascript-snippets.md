---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e680000fb85346872df28891fcb082fbf26b9386
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476802"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/onenote/notebooks')
    .version('beta')
    .get();

```