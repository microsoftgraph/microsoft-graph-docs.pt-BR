---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 409e20d77670896df7fb40eafeb6ebf8bdd582eb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335721"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let crossTenantAccessPolicyConfigurationPartner = await client.api('/policies/crossTenantAccessPolicy/partners/9c5d131d-b1c3-4fc4-9e3f-c6557947d551')
    .version('beta')
    .get();

```