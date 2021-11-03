---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f51222b6911ce8a34281220b3407b4272e945d6c
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60729973"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const passwordValidationInformation = {
    password: '1234567890'
};

await client.api('/users/validatePassword')
    .version('beta')
    .post(passwordValidationInformation);

```