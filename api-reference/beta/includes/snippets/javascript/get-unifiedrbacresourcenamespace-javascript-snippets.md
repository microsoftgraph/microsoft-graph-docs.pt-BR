---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0c81873f9783b6de373875a984e2ba49130e53c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338415"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRbacResourceNamespace = await client.api('/roleManagement/directory/resourceNamespaces/microsoft.aad.b2c')
    .version('beta')
    .get();

```