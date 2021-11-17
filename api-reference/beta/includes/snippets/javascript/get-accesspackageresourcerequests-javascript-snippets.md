---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 916768fb92e889d596e541c3eb6248afaabcc1c4dd7b7356d1318f34a6da0015
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898271"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageResourceRequests = await client.api('/identityGovernance/entitlementManagement/accessPackageResourceRequests')
    .version('beta')
    .get();

```