---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a38cc580adfa363503b63a16e283c3286e08fe46
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336624"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const crossTenantAccessPolicy = {
  displayName: 'CrossTenantAccessPolicy',
};

await client.api('/policies/crossTenantAccessPolicy')
    .version('beta')
    .update(crossTenantAccessPolicy);

```