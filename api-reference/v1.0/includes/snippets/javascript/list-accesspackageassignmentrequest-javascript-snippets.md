---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 469d349fb37f516b2480f583d910e9b0d2437f79
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342830"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentRequests = await client.api('/identityGovernance/entitlementManagement/assignmentRequests')
    .get();

```