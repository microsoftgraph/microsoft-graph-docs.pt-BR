---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3bd3c831ad317f19a1c48f2f05b553e1e9dbce8
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440075"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let cloudPcOverview = await client.api('/tenantRelationships/managedTenants/cloudPcsOverview/{cloudPcOverviewId}')
    .version('beta')
    .get();

```