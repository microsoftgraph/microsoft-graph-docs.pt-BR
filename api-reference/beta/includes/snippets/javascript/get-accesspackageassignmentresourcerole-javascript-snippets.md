---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70e46b7aef33ec62b00fe3d635e2c61cda4df383ed2123f8730ca7598fd8261e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099850"
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