---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d328b2881568f4fa4399f1ddd09e7c004037be5b56d9f48f9dbf62c2d4c04f99
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158777"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const tenantTag = {
  tenantIds: [
    'String'
  ]
};

await client.api('/tenantRelationships/managedTenants/tenantTags/{tenantTagId}/unassignTag')
    .version('beta')
    .post(tenantTag);

```