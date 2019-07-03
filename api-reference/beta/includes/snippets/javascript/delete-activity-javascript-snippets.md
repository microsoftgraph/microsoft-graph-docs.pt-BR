---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3a902150a96410d61e491c02cd1d16a1cf4ee08
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35475695"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/activities/13881113971988980728/')
    .version('beta')
    .delete();

```