---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 873258d36736b39443473342f43911afdf38bacc
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50797970"
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