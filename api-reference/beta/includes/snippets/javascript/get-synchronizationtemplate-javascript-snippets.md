---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d78dd342594f9b7f014c90586de47ef9efcd05c5
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35498790"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/synchronization/templates')
    .version('beta')
    .get();

```