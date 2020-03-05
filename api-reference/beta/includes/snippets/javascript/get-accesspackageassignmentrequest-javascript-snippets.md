---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84c37c39d0adf685ced8b7cc7da7bd1babec7c86
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "37992876"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}')
    .version('beta')
    .get();

```