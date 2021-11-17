---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f4bbecbfed54208144b879f62e43ca2e9d48c8d44c4855f9f04bc9f3f1453bbf
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898778"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentRequests = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests')
    .version('beta')
    .filter('(requestState eq \'PendingApproval\')')
    .expand('requestor($expand=connectedOrganization)')
    .get();

```