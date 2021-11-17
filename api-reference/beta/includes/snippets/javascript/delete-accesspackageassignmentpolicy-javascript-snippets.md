---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 163fd3465a859f3961e336518637a9ecb67638c053fd1f2b0d175894f79e2407
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}')
    .version('beta')
    .delete();

```