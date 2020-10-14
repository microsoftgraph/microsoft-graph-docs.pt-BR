---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5c9c73e6d2328e87542d4e3566b34b71a36665d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/14/2020
ms.locfileid: "48458125"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const emailAuthenticationMethod = {
  emailAddress: "kim@contoso.com"
};

let res = await client.api('/users/kim@contoso.com/authentication/emailMethods')
    .version('beta')
    .post(emailAuthenticationMethod);

```