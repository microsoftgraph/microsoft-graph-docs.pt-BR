---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad27ccbd8cadc7928fe493f333a46f9653eb0dd9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50789610"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentResourceRole = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles/{id}')
    .version('beta')
    .get();

```