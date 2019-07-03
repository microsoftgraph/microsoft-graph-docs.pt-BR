---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9bd2d6024438dffb75c384642dd83c8ae9844fce
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476193"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const validateCredentials = {
    credentials: [ 
        { key: "UserName", value: "user@domain.com" },
        { key: "Password", value: "password-value" }
    ]
};

let res = await client.api('/servicePrincipals/{id}/synchronization/jobs/{id}/validateCredentials')
    .version('beta')
    .post(validateCredentials);

```