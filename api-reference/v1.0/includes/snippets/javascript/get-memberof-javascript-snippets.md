---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad619386e45e976e531b7bec7ac9f69b7070202d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35492728"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/me/memberOf')
    .get();

```