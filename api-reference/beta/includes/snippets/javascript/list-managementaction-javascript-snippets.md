---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 18533f1b2a5ee2ecd67a1bafddc48db6b51183dd
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442455"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let managementActions = await client.api('/tenantRelationships/managedTenants/managementActions')
    .version('beta')
    .get();

```