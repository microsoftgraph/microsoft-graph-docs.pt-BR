---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5dac98282935e36d70514219b5bb2ac79e808bd2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475063"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const temporaryAccessPassAuthenticationMethod = {
  @odata.type: "#microsoft.graph.temporaryAccessPassAuthenticationMethod",
  startDateTime: "2021-01-26T00:00:00.000Z",
  lifetimeInMinutes: 60,
  isUsableOnce: false
};

let res = await client.api('/users/kim@contoso.com/authentication/temporaryAccessPassMethods')
    .version('beta')
    .post(temporaryAccessPassAuthenticationMethod);

```