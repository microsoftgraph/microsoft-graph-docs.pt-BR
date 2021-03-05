---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2fece1d5c226c2f00b273f1bd810a2aaad85733
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .get();

```