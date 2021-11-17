---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e54395579c149c4e0eb37ea752756f1380205602b2ea926a738a7698bed155dd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57159382"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/tenantRelationships/managedTenants/tenants/{tenantId}/resetTenantOnboardingStatus')
    .version('beta')
    .post();

```