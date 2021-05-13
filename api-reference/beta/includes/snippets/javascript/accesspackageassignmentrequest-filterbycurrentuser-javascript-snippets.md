---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 102113e7c2e3ac9b7547f2a2109f78520d36c3ea
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52473946"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let filterByCurrentUser = await client.api('/identityGovernance/entitlementManagement/accessPackages/filterByCurrentUser(on='allowedRequestor')')
    .version('beta')
    .get();

```