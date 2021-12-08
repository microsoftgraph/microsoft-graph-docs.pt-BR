---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4c9d82225e3963fffaacb6cde476a762c44c9da
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334554"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}')
    .delete();

```