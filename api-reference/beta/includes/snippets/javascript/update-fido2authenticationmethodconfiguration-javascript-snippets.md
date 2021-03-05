---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3b232557a8243bb33dbcbe2b7fcae5971210ae2
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471062"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const authenticationMethodConfiguration = {
    @odata.type: "#microsoft.graph.fido2AuthenticationMethodConfiguration",
    state: "enabled",
    isAttestationEnforced: "true"
};

let res = await client.api('/policies/authenticationMethodsPolicy/authenticationMethodConfigurations/fido2')
    .version('beta')
    .update(authenticationMethodConfiguration);

```