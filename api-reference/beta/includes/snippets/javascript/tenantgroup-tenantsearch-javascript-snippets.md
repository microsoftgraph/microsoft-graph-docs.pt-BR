---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0fff1da8eb6c555d60147d02e46fc9b3cf1367fc91889c0a3e3998086bb63f3a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898016"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantGroup = {
  tenantId: 'String'
};

await client.api('/tenantRelationships/managedTenants/tenantGroups/tenantSearch')
    .version('beta')
    .post(tenantGroup);

```