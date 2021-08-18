---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1fcd8d5f96b7458a382315f083a0c868bad4d4cf
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259056"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/policies/appManagementPolicies/{id}')
    .version('beta')
    .delete();

```