---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe10d99a5d8fd541c3e4fbcb41a0b05881d70700
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805858"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const phoneAuthenticationMethod = {
  phoneNumber: "+1 2065555554",
  phoneType: "mobile",
};

let res = await client.api('/me/authentication/phoneMethods/3179e48a-750b-4051-897c-87b9720928f7')
    .version('beta')
    .put(phoneAuthenticationMethod);

```