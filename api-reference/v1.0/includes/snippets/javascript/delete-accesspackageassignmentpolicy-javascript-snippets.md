---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 67d905c4e19d9c30253bae1abe382fc71da680bd
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/assignmentPolicies/{accessPackageAssignmentPolicyId}')
    .delete();

```