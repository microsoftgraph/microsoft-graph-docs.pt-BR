---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 50b5e34cb755c41c55c877c4a6a42b551a970ed3
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58262495"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const appManagementPolicy = {
 '@odata.id':'https://graph.microsoft.com/beta/policies/appManagementPolicies/{id}'
};

await client.api('/applications/{id}/appManagementPolicies/$ref')
    .version('beta')
    .post(appManagementPolicy);

```