---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d8a011a2feb54c788a26ad915b2661ef9444af66
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50942567"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let steps = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps')
    .version('beta')
    .get();

```