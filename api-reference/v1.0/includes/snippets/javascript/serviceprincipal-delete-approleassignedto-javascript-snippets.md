---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7faa465f80bd2747d35508ff6acb1bb9c1b71480
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441098"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{resource-SP-id}/appRoleAssignedTo/{appRoleAssignment-id}')
    .delete();

```