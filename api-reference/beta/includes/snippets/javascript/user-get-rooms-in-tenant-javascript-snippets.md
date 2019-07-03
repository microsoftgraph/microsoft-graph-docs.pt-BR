---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ab52f9899b1df42a3adeb2c72b17f844b2b0fbfb
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498775"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/findRooms')
    .version('beta')
    .get();

```