---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 176edf77d26efa43ae3684460f1473fe7a505903
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61337924"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/assignmentRequests/{accessPackageAssignmentRequestId}/cancel')
    .post();

```