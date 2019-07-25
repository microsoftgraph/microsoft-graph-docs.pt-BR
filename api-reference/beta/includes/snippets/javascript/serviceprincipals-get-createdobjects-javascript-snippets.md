---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0014628864279b1bfe16cf7dbc48010d77399685
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870046"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/servicePrincipals/{id}/createdObjects')
    .version('beta')
    .get();

```