---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c2f572f6e5c1e74fa85be917a283c8faee01a6f1
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337910"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const accessPackageAssignmentRequest = {
    requestType: 'AdminRemove',
    assignment: {
     id: 'a6bb6942-3ae1-4259-9908-0133aaee9377'
    }
};

await client.api('/identityGovernance/entitlementManagement/assignmentRequests')
    .post(accessPackageAssignmentRequest);

```