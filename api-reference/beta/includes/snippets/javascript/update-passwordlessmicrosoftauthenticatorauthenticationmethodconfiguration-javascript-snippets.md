---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad5fc1e1c0cfd6fd3097cd1638b09560576d9358
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    @odata.type: "#microsoft.graph.passwordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration",
    state: "enabled"
};

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/passwordlessMicrosoftAuthenticator')
    .version('beta')
    .update(authenticationMethodConfiguration);

```