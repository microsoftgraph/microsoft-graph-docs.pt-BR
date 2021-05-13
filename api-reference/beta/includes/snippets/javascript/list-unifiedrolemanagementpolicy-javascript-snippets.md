---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ba41ca33b590524e1dd7569b94d8662833cc284b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473436"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicies = await client.api('/policies/roleManagementPolicies')
    .version('beta')
    .get();

```