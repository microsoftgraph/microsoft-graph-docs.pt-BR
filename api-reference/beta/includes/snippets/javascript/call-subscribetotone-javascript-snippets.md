---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 002e323890cbd2bef7e8c5ee76823d563877e3f8
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35518718"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const CommsOperation = {
  clientContext: "d45324c1-fcb5-430a-902c-f20af696537c"
};

let res = await client.api('/app/calls/{id}/subscribeToTone')
    .version('beta')
    .post(CommsOperation);

```