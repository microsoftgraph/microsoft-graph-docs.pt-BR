---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 02097aea041aa88e466867db0b4887a4e526a1a7924e73e8567685f7ec896620
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099837"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResourceEnvironment = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceEnvironments/{accessPackageResourceEnvironmentId}')
    .version('beta')
    .get();

```