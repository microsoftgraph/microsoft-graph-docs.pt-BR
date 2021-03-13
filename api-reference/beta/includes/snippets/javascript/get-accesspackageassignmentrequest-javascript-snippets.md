---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7a7da9f1d7b96a3ffbcb52025f4330472035bf41
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808242"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let accessPackageAssignmentRequest = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}')
    .version('beta')
    .get();

```