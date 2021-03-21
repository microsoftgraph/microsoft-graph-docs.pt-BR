---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efacaf505b7ba264cee0b9c3ad002e11ec20acf0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960570"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentMultiple = await client.api('/roleManagement/deviceManagement/roleAssignments/lAPpYvVpN0KRkAEhdxReEJC2sEqbR_9Hr48lds9SGHI-1')
    .version('beta')
    .expand('directoryScopes')
    .get();

```