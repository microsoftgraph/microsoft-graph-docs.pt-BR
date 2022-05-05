---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a1256443a9c06091c48e2dfcd394da48ee07a08f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209680"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let assignmentPolicies = await client.api('/identityGovernance/entitlementManagement/assignmentPolicies')
    .get();

```