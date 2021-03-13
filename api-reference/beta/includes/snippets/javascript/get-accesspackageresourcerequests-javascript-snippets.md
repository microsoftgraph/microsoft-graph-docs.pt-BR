---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97ef19c6360f439c66349a4c9f1e24f2437faf4b
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50804933"
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