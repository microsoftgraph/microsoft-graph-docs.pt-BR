---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66484697d203ff65ce3fd30623f7b6e29bdcb3f4
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442487"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenant = await client.api('/tenantRelationships/managedTenants/tenants/{tenantId}')
    .version('beta')
    .get();

```