---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e21b84c0e8c1161cf09b296e021a6cb73fe4ccff
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473974"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  id: 'request-id',
  requestStatus: 'cancelled'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel')
    .version('beta')
    .post(cancel);

```