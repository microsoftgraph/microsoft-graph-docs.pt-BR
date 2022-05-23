---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de9ebb4d6e67fc3741b5066e803112067408da61
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629025"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let tenantUsage = await client.api('/tenantRelationships/managedTenants/tenantUsage')
    .version('beta')
    .get();

```